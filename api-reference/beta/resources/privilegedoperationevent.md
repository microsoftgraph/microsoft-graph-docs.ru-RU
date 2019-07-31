---
title: Тип ресурса Привилежедоператионевент
description: Представляет событие аудита, созданное с помощью привилегированного управления удостоверениями для операций с ролями, например администратором, который управляет привилегированными ролями, пользователь активирует свою роль, а пользователь отключает свою роль.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 88cc7870ef8db503dd2d0fd5f5de93ddf51bdac4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965763"
---
# <a name="privilegedoperationevent-resource-type"></a>Тип ресурса Привилежедоператионевент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет событие аудита, созданное с помощью привилегированного управления удостоверениями для операций с ролями, например администратором, который управляет привилегированными ролями, пользователь активирует свою роль, а пользователь отключает свою роль.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление privilegedOperationEvent](../api/privilegedoperationevent-list.md) | Коллекция [привилежедоператионевент](privilegedoperationevent.md) . |Получение коллекции объектов Привилежедоператионевент.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Аддитионалинформатион|string|Подробные сведения о событии, читаемые человеком.|
|Креатиондатетиме|dateTimeOffset|Указывает время создания события.|
|expirationDateTime|dateTimeOffset|Используется, только если значение requestType — "Activate", и оно указывает срок действия для активации роли.|
|id|string|Уникальный идентификатор для Привилежедоператионевент. Только для чтения.|
|Референцекэй|string|Номер билета инцидента или запроса во время активации роли. Значение отображается только в том случае, если номер билета предоставляется во время активации роли.|
|Референцесистем|string|Система билетов на инциденты и запросы, предоставляемая при активации Толе. Значение отображается только в том случае, если система билетов предоставляется во время активации роли.|
|requestType|string|Тип операции запроса. Значение requestType может принимать следующие значения ```Assign``` : (назначение ```Activate``` ролей), (активация ролей) ```Unassign``` , (удаление назначения роли) ```Deactivate``` , ( ```ScanAlersNow``` отключение уведомлений ```DismissAlert``` системы безопасности), (отклонить оповещение системы безопасности) ( ```FixAlertItem``` исправить безопасность) (исправить безопасность предупреждение об ошибке ```AccessReview_Review``` ), (обзор проверки доступа) ```AccessReview_Create``` , (создание проверки доступа), ```AccessReview_Update``` (обновление проверки доступа) и ```AccessReview_Delete``` (удаление проверки доступа).|
|Рекуесторид|string|Идентификатор пользователя запрашивающего, который инициирует операцию.|
|Рекуесторнаме|string|Имя пользователя запрашивающего, который инициирует операцию.|
|roleId|string|Идентификатор роли, связанной с операцией.|
|roleName|string|Имя роли.|
|tenantId|string|Идентификатор клиента (организации).|
|userId|string|Идентификатор пользователя, связанного с операцией.|
|Усермаил|string|Адрес электронной почты пользователя.|
|userName|string|Отображаемое имя пользователя.|

## <a name="relationships"></a>Отношения
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
  "userName": "string",
  "referenceKey": "string",
  "referenceSystem": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
