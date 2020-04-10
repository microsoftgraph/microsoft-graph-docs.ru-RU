---
title: Тип ресурса Привилежедоператионевент
description: Представляет событие аудита, созданное с помощью привилегированного управления удостоверениями для операций с ролями, например администратором, который управляет привилегированными ролями, пользователь активирует свою роль, а пользователь отключает свою роль.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 7c98b26d6c6b3458bddc8c5bf5f567f1002d082a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219202"
---
# <a name="privilegedoperationevent-resource-type"></a>Тип ресурса Привилежедоператионевент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет событие аудита, созданное с помощью привилегированного управления удостоверениями для операций с ролями, например администратором, который управляет привилегированными ролями, пользователь активирует свою роль, а пользователь отключает свою роль.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление privilegedOperationEvent](../api/privilegedoperationevent-list.md) | Коллекция [привилежедоператионевент](privilegedoperationevent.md) . |Получение коллекции объектов Привилежедоператионевент.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|аддитионалинформатион|string|Подробные сведения о событии, читаемые человеком.|
|креатиондатетиме|dateTimeOffset|Указывает время создания события.|
|expirationDateTime|dateTimeOffset|Используется, только если значение requestType — "Activate", и оно указывает срок действия для активации роли.|
|id|string|Уникальный идентификатор для Привилежедоператионевент. Только для чтения.|
|референцекэй|string|Номер билета инцидента или запроса во время активации роли. Значение отображается только в том случае, если номер билета предоставляется во время активации роли.|
|референцесистем|string|Система билетов на инциденты и запросы, предоставляемая при активации Толе. Значение отображается только в том случае, если система билетов предоставляется во время активации роли.|
|requestType|string|Тип операции запроса. Значение requestType может быть следующим: ```Assign``` ( ```Activate``` назначение ролей), (Активация роли), ```Unassign``` (удаление назначения роли), ```Deactivate``` (деактивация ```ScanAlersNow``` роли), (предупреждение системы безопасности при сканировании ```DismissAlert``` ), (предупреждение ```FixAlertItem``` системы безопасности) (устранение проблемы с оповещением системы безопасности), (устранение проблемы ```AccessReview_Review``` с оповещением системы безопасности), (изучите проверку ```AccessReview_Create``` доступа), (создать проверку ```AccessReview_Update``` доступа), (обновить ```AccessReview_Delete```|
|рекуесторид|string|Идентификатор пользователя запрашивающего, который инициирует операцию.|
|рекуесторнаме|string|Имя пользователя запрашивающего, который инициирует операцию.|
|roleId|string|Идентификатор роли, связанной с операцией.|
|roleName|string|Имя роли.|
|tenantId|string|Идентификатор клиента (организации).|
|userId|строка|Идентификатор пользователя, связанного с операцией.|
|усермаил|string|Адрес электронной почты пользователя.|
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
