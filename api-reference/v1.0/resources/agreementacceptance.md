---
title: тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с Azure Active Directory Azure AD.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: fe3d453c7cbd34586bd8db2aaa812cd2a864fa8d
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451021"
---
# <a name="agreementacceptance-resource-type"></a>тип ресурса agreementAcceptance

Пространство имен: microsoft.graph

Представляет текущее состояние ответа пользователя на настраиваемые условия соглашения об использовании компании с Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|agreementFileId|String|Идентификатор файла соглашения, принятого пользователем.|
|agreementId|String|Идентификатор соглашения.|
|deviceDisplayName|String|Отображающее имя устройства, используемого для  принятие соглашения.|
|deviceId|String|Уникальный идентификатор устройства, используемого для  принятие соглашения.|
|deviceOSType|String|Операционная система, используемая для  принятие соглашения.|
|deviceOSVersion|String|Версия операционной системы устройства, используемая для  принятие соглашения.    |
|expirationDateTime|DateTimeOffset|Срок действия даты принятия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String| Идентификатор принятия соглашения. Только для чтения.|
|recordedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|состояние|string| Состояние принятия соглашения. Возможные значения: `accepted`, `declined`. Поддерживает `$filter` (`eq`).|
|userDisplayName|String|Отображение имени пользователя при записи приемки.|
|userEmail|String|Электронная почта пользователя при записи принятия.|
|userId|String|Идентификатор пользователя, который принял соглашение.|
|userPrincipalName|String|UPN пользователя при записи принятия.|

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


