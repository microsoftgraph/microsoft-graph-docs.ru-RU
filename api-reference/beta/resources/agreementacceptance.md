---
title: Тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 18bcf00cad681d3003faf2dce442e4ea1f58bdb0
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643981"
---
# <a name="agreementacceptance-resource-type"></a>Тип ресурса agreementAcceptance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|агриментфилеид|String|Идентификатор файла соглашения, принятого пользователем.|
|агриментид|String|Идентификатор соглашения.|
|deviceDisplayName|String|Отображаемое имя устройства, используемое для принятия соглашения.|
|deviceId|String|Уникальный идентификатор устройства, используемого для принятия соглашения.|
|девицеостипе|String|Операционная система, используемая для принятия соглашения.|
|девицеосверсион|String|Версия операционной системы устройства, используемая для принятия соглашения.    |
|expirationDateTime|DateTimeOffset|Дата и время окончания срока действия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|recordedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|состояние|string| Возможные значения: `accepted`, `declined`.|
|userDisplayName|String|Отображаемое имя пользователя, когда оно было записано.|
|userEmail|String|Сообщение электронной почты пользователя, когда сообщение о принятии было записано.|
|userId|String|Идентификатор пользователя, который принял соглашение.|
|userPrincipalName|String|Имя участника-пользователя, когда оно было записано.|

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
      "id": "String (identifier)",
      "agreementId": "String",
      "userId": "String",
      "deviceId": "String",
      "deviceDisplayName": "String",
      "deviceOSType": "String",
      "deviceOSVersion": "String",
      "agreementFileId": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userEmail": "String",
      "recordedDateTime": "String (timestamp)",
      "expirationDateTime": "String",
      "state": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
