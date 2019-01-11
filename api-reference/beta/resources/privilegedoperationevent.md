---
title: Тип ресурса privilegedOperationEvent
description: Представляет событие аудита, созданное привилегированной управления удостоверениями для операций роли, такие как администратор управляет привилегированной ролей, пользователь активирует его роли и пользователь деактивирует его роль.
localization_priority: Normal
ms.openlocfilehash: cc7374f4cf3bc18fbf2f3c36ee4f57e6d703434b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882686"
---
# <a name="privilegedoperationevent-resource-type"></a>Тип ресурса privilegedOperationEvent

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет событие аудита, созданное привилегированной управления удостоверениями для операций роли, такие как администратор управляет привилегированной ролей, пользователь активирует его роли и пользователь деактивирует его роль.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список privilegedOperationEvent](../api/privilegedoperationevent-list.md) | Коллекция [privilegedOperationEvent](privilegedoperationevent.md) . |Получите коллекцию объектов privilegedOperationEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|string|Подробные человеческого для чтения сведения для события.|
|creationDateTime|dateTimeOffset|Указывает время создания события.|
|expirationDateTime|dateTimeOffset|Используется, только когда requestType «Активировать» и ее указывает время истечения срока действия для активации роли.|
|id|строка|Уникальный идентификатор для privilegedOperationEvent. Только для чтения.|
|referenceKey|string|Номер происшествия/запроса билетов во время активации роли. Значение предоставляется только в том случае, если номер билетов предоставляется во время активации роли.|
|referenceSystem|string|Происшествие/запрос, полученное во время активации tole система отслеживания ошибок. Значение предоставляется только в том случае, если во время активации роли предоставляется система билетов.|
|requestType|string|Тип операции запроса. Значение requestType может быть: ```Assign``` (назначение), ```Activate``` (роль активации), ```Unassign``` (удалить назначения роли), ```Deactivate``` (роль деактивации), ```ScanAlersNow``` (сканирование оповещение системы безопасности), ```DismissAlert``` (отключить оповещение системы безопасности), ```FixAlertItem``` (исправления безопасности предупреждения проблема), ```AccessReview_Review``` (просмотрите доступа, просмотрите), ```AccessReview_Create``` (создать доступа, просмотрите), ```AccessReview_Update``` (Обновить доступа, просмотрите), и ```AccessReview_Delete``` (удаление доступа, просмотрите).|
|requestorId|string|Идентификатор инициатора запроса, который запускает операцию.|
|requestorName|string|Имя пользователя, запрашивающего, инициирующий операции.|
|roleId|string|Идентификатор роли, связанное с операцией.|
|Имя роли|string|Имя роли.|
|tenantId|string|Идентификатор клиента (организация).|
|userId|string|Идентификатор пользователя, который связан с операцией.|
|userMail|string|Адреса электронной почты пользователя.|
|userName|string|Отображаемое имя пользователя.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}-->

```json
{
  "additionalInformation": "string",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "requestType": "string",
  "requestorId": "string",
  "requestorName": "string",
  "roleId": "string",
  "roleName": "string",
  "tenantId": "string",
  "userId": "string",
  "userMail": "string",
  "userName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
