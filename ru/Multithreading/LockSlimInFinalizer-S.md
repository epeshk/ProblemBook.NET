# «LockSlimInFinalizer» (Решение)

## Ответ

```
~Foo: start
Exception: SynchronizationLockException
~Foo: finish
```

## Объяснение

Произойдёт [SynchronizationLockException](http://msdn.microsoft.com/library/system.threading.synchronizationlockexception.aspx), т.к. финализатор будет вызван сборщиком мусора, который работает в другом потоке.

[Задача](./LockSlimInFinalizer-P.md)