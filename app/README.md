# app

A new Flutter project.

## Getting Started

For help getting started with Flutter, view our online
[documentation](https://flutter.io/).



##bugfix:
- 1.in flare_flutter/base -->  actor_ik_constraint.dart --> void solve2(BoneChain fk1, BoneChain fk2, Vec2D worldTargetTranslation)
> - RangeError (index): Invalid value: Not in inclusive range 0..1: 11，Because _fkChain.length is Always 2
> - Unhandled Exception: RangeError (index): Invalid value: Not in inclusive range 0..1: 11
> - #0      List.[] (dart:core-patch/growable_array.dart:254:60)
> - #1      ActorIKConstraint.solve2 (package:flare_flutter/base/actor_ik_constraint.dart:256:36)
> - #2      ActorIKConstraint.constrain (package:flare_flutter/base/actor_ik_constraint.dart:133:7)
- 2.in flare_flutter/base --> actor_artboard.dart --> void advance(double seconds)
> _dependencyOrder is Always unNull but _dependencyOrder![i] may be null
> - The following _CastError was thrown building Container(constraints: BoxConstraints(0.0<=w<=Infinity, h=280.0)):
Null check operator used on a null value
> - The relevant error-causing widget was:
> -   Container file:///[Project dir]/lib/article/article_widget.dart:165:40
> - When the exception was thrown, this was the stack:
> - #0      ActorArtboard.advance (package:flare_flutter/base/actor_artboard.dart:326:62)
> - #1      VignetteRenderObject.updateActor (package:the_history_of_everything/article/timeline_entry_widget.dart:108:21)
> _dependencyOrder![i]!