# ASCII Flowchart Drawing Cheat Sheet

## Basic Shapes

### Process
```text
+-----------+
|  Process  |
+-----------+
```

### Start / End
```text
 .--------.
(  Start  )
 '--------'
```

```text
 .------.
(  End  )
 '------'
```

### Decision
```text
    /-----\\
   / Yes?  \\
   \\       /
    \\-----/
```

## Arrows

```text
A -----> B

A
|
v
B

A <----> B
```

## Simple Flow

```text
 .-------.
( Start )
 '---+---'
     |
     v
+---------+
| Process |
+----+----+
     |
     v
 .-----.
( End )
 '-----'
```

## Decision Branch

```text
+---------+
| Process |
+----+----+
     |
     v
 +-------+
 | Valid?|
 +---+---+
     |
  +--+--+
  |     |
Yes     No
  |     |
  v     v
+---+ +------+
| OK| |Retry |
+---+ +------+
```

## Loop

```text
+---------+
| Process |
+----+----+
     |
     v
+---------+
| More ?  |
+----+----+
     |
  Yes|-----+
     |     |
     v     |
+---------+|
| Process ||
+---------+|
     ^     |
     +-----+
```

## Tree

```text
Root
 |
 +--Child A
 |
 +--Child B
 |   |
 |   +--Sub B1
 |   +--Sub B2
 |
 +--Child C
```

## Unicode Box Drawing

```text
┌─────────┐
│ Process │
└─────────┘
```

### Connectors

```text
│ Vertical
─ Horizontal
┌ ┐ └ ┘ Corners
├ ┤ Junctions
┬ ┴ Tees
┼ Cross
```

## Professional Example

```text
┌─────────┐
│  Start  │
└────┬────┘
     │
     ▼
┌─────────┐
│  Input  │
└────┬────┘
     │
     ▼
┌─────────┐
│Validate │
└────┬────┘
     │
     ▼
   ┌─────┐
   │ OK? │
   └──┬──┘
      │
   ┌──┴──┐
   │     │
 Yes     No
   │     │
   ▼     ▼
┌─────┐ ┌─────┐
│Save │ │Error│
└──┬──┘ └──┬──┘
   │        │
   └──┬─────┘
      ▼
┌─────────┐
│   End   │
└─────────┘
```

## Quick Reference

```text
[] Process
() Start/End
<> Decision
{} Grouping
| Vertical
- Horizontal
+ Junction
> Arrow
```
