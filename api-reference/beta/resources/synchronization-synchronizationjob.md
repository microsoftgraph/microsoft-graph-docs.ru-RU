---
title: Тип ресурса synchronizationJob
description: Выполняет синхронизацию путем периодического выполнения в фоновом режиме, опроса изменений в одном каталоге и их перенанесения в другой каталог.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 0f0036cd26a72effba41085d9a4638647fd4060e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132043"
---
# <a name="synchronizationjob-resource-type"></a>Тип ресурса synchronizationJob

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Выполняет синхронизацию путем периодического выполнения в фоновом режиме, опроса изменений в одном каталоге и их перенанесения в другой каталог. Задание синхронизации всегда является специфическим для конкретного экземпляра приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге и настроить схему синхронизации задания.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[Список](../api/synchronization-synchronizationjob-list.md)             |[Коллекция synchronizationJob](synchronization-synchronizationjob.md)  |Список существующих заданий для заданного экземпляра приложения (участников-служб).|
|[Get synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |Чтение свойств и связей объекта synchronizationJob.|
|[Создание](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |Создайте новое задание для заданного приложения.|
|[Начало](../api/synchronization-synchronizationjob-start.md)          |Нет   |Запустите синхронизацию. Если задание приостановлено, оно продолжается с момента приостановки задания. Если задание находится в карантине, состояние карантина очищается.|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |Нет   |При принудительном запуске задания и повторной обработке всех объектов в каталоге.|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |Нет   |Временно остановите синхронизацию. Все ходы выполнения, включая состояние задания, сохраняются, и задание продолжит работу с того места, где оно было отключено при [запуске](../api/synchronization-synchronizationjob-start.md) вызова.|
|[Delete](../api/synchronization-synchronizationjob-delete.md)        |Нет   |Остановите синхронизацию и окончательно удалите все состояние, связанное с заданием.|
|[Get synchronizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Получить эффективную схему синхронизации задания.|
|[Обновление synchronizationSchema](../api/synchronization-synchronizationschema-update.md)    |Нет   |Обновление схемы синхронизации задания. |
|[Проверка учетных данных](../api/synchronization-synchronizationjob-validatecredentials.md)|Нет|Проверьте предоставленные учетные данные в целевом каталоге.|
|[provisionOnDemand](../api/synchronization-synchronizationjob-provision-on-demand.md)|[Коллекция synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md)|Представляет объекты, которые будут быть выполнены с выполнением правил синхронизации. Ресурс в основном используется для предоставления по требованию. |
## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|id             |Строка                     |Уникальный идентификатор задания синхронизации. Только для чтения.|
|schedule       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|Расписание, используемая для запуска задания. Только для чтения.|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.|
|synchronizationJobSettings   |[keyValuePair](keyvaluepair.md);    |Параметры, связанные с заданием. Некоторые параметры наследуются от шаблона.|
|templateId     |Строка    |Идентификатор шаблона [синхронизации, на](synchronization-synchronizationtemplate.md) котором основано это задание.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|схема|[synchronizationSchema](synchronization-synchronizationschema.md)| Схема синхронизации, настроенная для задания.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "synchronizationJobSettings": {"@odata.type": "microsoft.graph.keyValuePair"},
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
  "suppressions": []
}
-->


