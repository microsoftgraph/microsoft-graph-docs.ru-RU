---
title: Тип ресурса synchronizationJob
description: Выполняет синхронизацию с периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог. Задание синхронизации всегда специально для конкретного экземпляра приложения клиента. Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510570"
---
# <a name="synchronizationjob-resource-type"></a>Тип ресурса synchronizationJob

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|Расписание       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|Расписание выполнения задания. Только для чтения.|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |Состояние задания, которое включает в себя после последнего выполнения задания, текущее состояние задания и ошибках.|
|templateId     |String    |Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) на основе этого задания.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjob.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
