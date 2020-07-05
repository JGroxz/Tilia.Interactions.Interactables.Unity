# Class TouchInteractableConfigurator

## Contents

* [Inheritance]
* [Namespace]
* [Syntax]
* [Fields]
  * [touchingInteractors]
* [Properties]
  * [AddActiveInteractor]
  * [CurrentTouchingObjects]
  * [Facade]
  * [PotentialInteractors]
  * [RemoveActiveInteractor]
  * [TouchConsumer]
  * [TouchingInteractors]
  * [TouchValidity]
  * [UntouchConsumer]
* [Methods]
  * [ConfigureContainer()]
  * [GetTouchingInteractors()]
  * [LinkActiveInteractorCollisions()]
  * [NotifyTouch(GameObject)]
  * [NotifyUntouch(GameObject)]
  * [OnDisable()]
  * [OnEnable()]
  * [ProcessPotentialInteractorContentChange(CollisionNotifier.EventData)]
  * [UnlinkActiveInteractorCollisions()]

## Details

##### Inheritance

* System.Object
* TouchInteractableConfigurator

##### Namespace

* [Tilia.Interactions.Interactables.Interactables.Touch]

##### Syntax

```
public class TouchInteractableConfigurator : MonoBehaviour
```

### Fields

#### touchingInteractors

A reusable collection to hold the returned touching interactors.

##### Declaration

```
protected readonly List<InteractorFacade> touchingInteractors
```

### Properties

#### AddActiveInteractor

The NotifierContainerExtractor for adding active interactors.

##### Declaration

```
public NotifierContainerExtractor AddActiveInteractor { get; protected set; }
```

#### CurrentTouchingObjects

The GameObjectObservableList that holds the current touching objects data.

##### Declaration

```
public GameObjectObservableList CurrentTouchingObjects { get; protected set; }
```

#### Facade

The public interface facade.

##### Declaration

```
public InteractableFacade Facade { get; protected set; }
```

#### PotentialInteractors

The ActiveCollisionsContainer for potential interactors.

##### Declaration

```
public ActiveCollisionsContainer PotentialInteractors { get; protected set; }
```

#### RemoveActiveInteractor

The NotifierContainerExtractor for removing active interactors.

##### Declaration

```
public NotifierContainerExtractor RemoveActiveInteractor { get; protected set; }
```

#### TouchConsumer

The ActiveCollisionConsumer that listens for the touch payload.

##### Declaration

```
public ActiveCollisionConsumer TouchConsumer { get; protected set; }
```

#### TouchingInteractors

A collection of Interactors that are currently touching the Interactable.

##### Declaration

```
public IReadOnlyList<InteractorFacade> TouchingInteractors { get; }
```

#### TouchValidity

The GameObjectEventProxyEmitter used to determine the touch validity.

##### Declaration

```
public GameObjectEventProxyEmitter TouchValidity { get; protected set; }
```

#### UntouchConsumer

The ActiveCollisionConsumer that listens for the untouch payload.

##### Declaration

```
public ActiveCollisionConsumer UntouchConsumer { get; protected set; }
```

### Methods

#### ConfigureContainer()

Sets the consumer containers to the current active container.

##### Declaration

```
public virtual void ConfigureContainer()
```

#### GetTouchingInteractors()

Retrieves a collection of Interactors that are touching the Interactable.

##### Declaration

```
protected virtual IReadOnlyList<InteractorFacade> GetTouchingInteractors()
```

##### Returns

| Type | Description |
| --- | --- |
| System.Collections.Generic.IReadOnlyList<[InteractorFacade]\> | The touching Interactors. |

#### LinkActiveInteractorCollisions()

Links the CollisionNotifier to the potential and active interactor logic.

##### Declaration

```
protected virtual void LinkActiveInteractorCollisions()
```

#### NotifyTouch(GameObject)

Notifies that the Interactable is being touched.

##### Declaration

```
public virtual void NotifyTouch(GameObject data)
```

##### Parameters

| Type | Name | Description |
| --- | --- | --- |
| GameObject | data | The touching object. |

#### NotifyUntouch(GameObject)

Notifies that the Interactable is being no longer touched.

##### Declaration

```
public virtual void NotifyUntouch(GameObject data)
```

##### Parameters

| Type | Name | Description |
| --- | --- | --- |
| GameObject | data | The previous touching object. |

#### OnDisable()

##### Declaration

```
protected virtual void OnDisable()
```

#### OnEnable()

##### Declaration

```
protected virtual void OnEnable()
```

#### ProcessPotentialInteractorContentChange(CollisionNotifier.EventData)

Handles any change of collision contents.

##### Declaration

```
protected virtual void ProcessPotentialInteractorContentChange(CollisionNotifier.EventData data)
```

##### Parameters

| Type | Name | Description |
| --- | --- | --- |
| CollisionNotifier.EventData | data | The changed collision data. |

#### UnlinkActiveInteractorCollisions()

Unlinks the CollisionNotifier to the potential and active interactor logic.

##### Declaration

```
protected virtual void UnlinkActiveInteractorCollisions()
```

[Tilia.Interactions.Interactables.Interactables.Touch]: README.md
[InteractorFacade]: ../../Interactors/InteractorFacade.md
[InteractableFacade]: ../../Interactables/InteractableFacade.md
[Inheritance]: #Inheritance
[Namespace]: #Namespace
[Syntax]: #Syntax
[Fields]: #Fields
[touchingInteractors]: #touchingInteractors
[Properties]: #Properties
[AddActiveInteractor]: #AddActiveInteractor
[CurrentTouchingObjects]: #CurrentTouchingObjects
[Facade]: #Facade
[PotentialInteractors]: #PotentialInteractors
[RemoveActiveInteractor]: #RemoveActiveInteractor
[TouchConsumer]: #TouchConsumer
[TouchingInteractors]: #TouchingInteractors
[TouchValidity]: #TouchValidity
[UntouchConsumer]: #UntouchConsumer
[Methods]: #Methods
[ConfigureContainer()]: #ConfigureContainer
[GetTouchingInteractors()]: #GetTouchingInteractors
[LinkActiveInteractorCollisions()]: #LinkActiveInteractorCollisions
[NotifyTouch(GameObject)]: #NotifyTouchGameObject
[NotifyUntouch(GameObject)]: #NotifyUntouchGameObject
[OnDisable()]: #OnDisable
[OnEnable()]: #OnEnable
[ProcessPotentialInteractorContentChange(CollisionNotifier.EventData)]: #ProcessPotentialInteractorContentChangeCollisionNotifier.EventData
[UnlinkActiveInteractorCollisions()]: #UnlinkActiveInteractorCollisions