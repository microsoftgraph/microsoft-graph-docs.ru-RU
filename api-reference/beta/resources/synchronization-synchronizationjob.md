---
title: Тип ресурса synchronizationJob
description: Выполняет синхронизацию с периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог. Задание синхронизации всегда специально для конкретного экземпляра приложения клиента. Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.
ms.openlocfilehash: 0e6428f2a088e5326f4412e743489c4d94b10296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082245"
---
# <a name="synchronizationjob-resource-type"></a>Тип ресурса synchronizationJob

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Выполняет синхронизацию с периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог. Задание синхронизации всегда специально для конкретного экземпляра приложения клиента. Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[synchronizationJob](synchronization-synchronizationjob.md) коллекции  |Список существующих заданий для экземпляра данного приложения (участников-служб).|
|[Получение synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |Чтение свойства и связи объекта synchronizationJob.|
|[Create](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |Создание нового задания для данного приложения.|
|[Start](../api/synchronization-synchronizationjob-start.md)          |Нет   |Запуск синхронизации. Если задание находится в приостановленном состоянии, он по-прежнему производится из точки, где был приостановлен задания. Если задание находится в карантине, состояние карантина снят.|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |Нет   |Принудительное задание, чтобы начать заново и повторно обрабатывать все объекты в каталоге.|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |Нет   |Временно приостановить синхронизации. Сохраняются все текущие, включая состояние задания и задание продолжит работу с где оно было прервано Если [запустить](../api/synchronization-synchronizationjob-start.md) вызов.|
|[Delete](../api/synchronization-synchronizationjob-delete.md)        |Нет   |Остановите синхронизацию и окончательно удалить все состояния, связанных с заданием.|
|[Получение synchrnoizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Получите схему эффективной синхронизации задания.|
|[Обновление synchroizationSchema](../api/synchronization-synchronizationschema-update.md)    |Нет   |Обновление схемы заданий синхронизации. |
|[Проверка учетных данных](../api/synchronization-synchronizationjob-validatecredentials.md)|Нет|Тестирование предоставленные учетные данные для целевой каталог.|

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|id             |String                     |Идентификатор задания уникальных синхронизации. Только для чтения.|
|расписание       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|Расписание выполнения задания. Только для чтения.|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |Состояние задания, которое включает в себя после последнего выполнения задания, текущее состояние задания и ошибках.|
|templateId     |String    |Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) на основе этого задания.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Description|
|:---------------|:--------|:----------|
|схема|[synchronizationSchema](synchronization-synchronizationschema.md)| Схема синхронизации, настроенных для задания.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->