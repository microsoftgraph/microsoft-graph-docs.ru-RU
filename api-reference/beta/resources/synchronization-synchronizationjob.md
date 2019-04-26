---
title: Тип ресурса Синчронизатионжоб
description: Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог. Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.
localization_priority: Normal
ms.openlocfilehash: 43563de6e6ca88eac63b4f4b4bc4afd3fb78abc3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345701"
---
# <a name="synchronizationjob-resource-type"></a>Тип ресурса Синчронизатионжоб

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог. Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[Перечисление](../api/synchronization-synchronizationjob-list.md)             |Коллекция [синчронизатионжоб](synchronization-synchronizationjob.md)  |ПереЧисление существующих заданий для определенного экземпляра приложения (субъекта-службы).|
|[Получение Синчронизатионжоб](../api/synchronization-synchronizationjob-get.md) | [Синчронизатионжоб](synchronization-synchronizationjob.md) |Чтение свойств и связей объекта Синчронизатионжоб.|
|[Создание](../api/synchronization-synchronizationjob-post.md)         |[Синчронизатионжоб](synchronization-synchronizationjob.md)   |Создание нового задания для определенного приложения.|
|[Start](../api/synchronization-synchronizationjob-start.md)          |Нет   |Запуск синхронизации. Если задание приостановлено, оно продолжается с того места, где было приостановлено задание. Если задание находится в карантине, статус карантина очищается.|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |Нет   |Принудительно запустить задание и повторно обработать все объекты в каталоге.|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |Нет   |Временная остановка синхронизации. Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.|
|[Удаление](../api/synchronization-synchronizationjob-delete.md)        |Нет   |Остановите синхронизацию и окончательно удалите все состояния, связанные с заданием.|
|[Получение Синчрноизатионсчема](../api/synchronization-synchronizationschema-get.md)    |[Синчронизатионсчема](synchronization-synchronizationschema.md)   |Получение действующей схемы синхронизации задания.|
|[Обновление Синчроизатионсчема](../api/synchronization-synchronizationschema-update.md)    |Нет   |Обновите схему синхронизации задания. |
|[Проверка учетных данных](../api/synchronization-synchronizationjob-validatecredentials.md)|Нет|Проверка предоставленных учетных данных в целевом каталоге.|

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|id             |String                     |Уникальный идентификатор задания синхронизации. Только для чтения.|
|Диспетчер       |[Синчронизатионсчедуле](synchronization-synchronizationschedule.md)|Расписание, используемое для запуска задания. Только для чтения.|
|status         |[Синчронизатионстатус](synchronization-synchronizationstatus.md)     |Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.|
|templateId     |String    |Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) , на котором основано это задание.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|схемы|[Синчронизатионсчема](synchronization-synchronizationschema.md)| Схема синхронизации, настроенная для задания.|

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
