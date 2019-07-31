---
title: Тип ресурса Синчронизатионжоб
description: Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог. Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a311c8ae7618778c2dbd8cdbc9a5b30af254eae4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007797"
---
# <a name="synchronizationjob-resource-type"></a>Тип ресурса Синчронизатионжоб

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог. Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |Коллекция [синчронизатионжоб](synchronization-synchronizationjob.md)  |Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).|
|[Получение Синчронизатионжоб](../api/synchronization-synchronizationjob-get.md) | [Синчронизатионжоб](synchronization-synchronizationjob.md) |Чтение свойств и связей объекта Синчронизатионжоб.|
|[создание](../api/synchronization-synchronizationjob-post.md);         |[Синчронизатионжоб](synchronization-synchronizationjob.md)   |Создание нового задания для определенного приложения.|
|[Start](../api/synchronization-synchronizationjob-start.md)          |Нет   |Запуск синхронизации. Если задание приостановлено, оно продолжается с того места, где было приостановлено задание. Если задание находится в карантине, статус карантина очищается.|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |Нет   |Принудительно запустить задание и повторно обработать все объекты в каталоге.|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |Нет   |Временная остановка синхронизации. Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.|
|[Удаление](../api/synchronization-synchronizationjob-delete.md)        |Нет   |Остановите синхронизацию и окончательно удалите все состояния, связанные с заданием.|
|[Получение Синчронизатионсчема](../api/synchronization-synchronizationschema-get.md)    |[Синчронизатионсчема](synchronization-synchronizationschema.md)   |Получение действующей схемы синхронизации задания.|
|[Обновление Синчронизатионсчема](../api/synchronization-synchronizationschema-update.md)    |Нет   |Обновите схему синхронизации задания. |
|[Проверка учетных данных](../api/synchronization-synchronizationjob-validatecredentials.md)|Нет|Проверка предоставленных учетных данных в целевом каталоге.|

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|id             |String                     |Уникальный идентификатор задания синхронизации. Только для чтения.|
|schedule       |[Синчронизатионсчедуле](synchronization-synchronizationschedule.md)|Расписание, используемое для запуска задания. Только для чтения.|
|status         |[Синчронизатионстатус](synchronization-synchronizationstatus.md)     |Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.|
|templateId     |String    |Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) , на котором основано это задание.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|схемы|[Синчронизатионсчема](synchronization-synchronizationschema.md)| Схема синхронизации, настроенная для задания.|

## <a name="json-representation"></a>Представление JSON

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
