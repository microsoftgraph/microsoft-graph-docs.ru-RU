---
title: тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 2df1803b8601635eba163aa3abd46d70ee0a5723
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089972"
---
# <a name="agreementacceptance-resource-type"></a>тип ресурса agreementAcceptance

Пространство имен: microsoft.graph

Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|agreementFileId|Строка|Идентификатор файла соглашения, принятого пользователем.|
|agreementId|Строка|Идентификатор соглашения.|
|deviceDisplayName|String|Отображающее имя устройства, используемого для принятие соглашения.|
|deviceId|String|Уникальный идентификатор устройства, используемого для принятие соглашения.|
|deviceOSType|Строка|Операционная система, используемая для принятие соглашения.|
|deviceOSVersion|Строка|Версия операционной системы устройства, используемая для принятие соглашения.    |
|expirationDateTime|DateTimeOffset|Срок действия даты принятия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|Строка| Идентификатор принятия соглашения. Только для чтения.|
|recordedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|состояние|string| Состояние принятия соглашения. Возможные значения: `accepted`, `declined`.|
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


