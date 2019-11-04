---
title: Тип ресурса Акцесспаккажеассигнмент
description: Назначение пакета Access — это назначение пакета Access определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 234aad48e11a2b6c5c2a47c494216fa15fbc139b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939217"
---
# <a name="accesspackageassignment-resource-type"></a>Тип ресурса Акцесспаккажеассигнмент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)назначение пакета Access — это назначение пакета доступа определенной теме в течение определенного периода времени.  Например, при назначении пакета доступа может быть задано, что пользователю "Алиса" назначен доступ через пакет Access "продажи" в течение периода с 2019 по 2019 июля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Акцесспаккажеассигнментс](../api/accesspackageassignment-list.md) | Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md) | Получение списка объектов **акцесспаккажеассигнмент** . |

>**Примечание:** Невозможно использовать метод для создания назначения пакета Access. Вместо этого клиент, которому требуется запросить назначение пакета доступа для пользователя, может [создать акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккажеид|Строка|Идентификатор пакета Access. Только для чтения.|
|ассигнментполициид|Строка|Идентификатор политики назначения пакетов доступа. Только для чтения.|
|ассигнментстате|String|Только для чтения.|
|Свойства assignmentstatus|String|Только для чтения.|
|каталогид|Строка|Идентификатор каталога, содержащего пакет Access. Только для чтения.|
|експиреддатетиме|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|Расширенная|Логический|Указывает, является ли назначение пакета доступа расширенным. Только для чтения.|
|targetId|Строка| ИДЕНТИФИКАТОР субъекта с назначением. Только для чтения.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккаже|[акцесспаккаже](accesspackage.md)| Только для чтения. Допускается значение null.|
|акцесспаккажеассигнментполици|[акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)| Только для чтения. Допускается значение null.|
|акцесспаккажеассигнментресаурцеролес|Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)| Только для чтения. Допускается значение null.|
|target|[акцесспаккажесубжект](accesspackagesubject.md)| Тема назначения пакета Access. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
            "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
            "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
            "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
            "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
            "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
            "assignmentStatus": "ExpiredNotificationTriggered",
            "assignmentState": "Expired",
            "isExtended": false,
            "expiredDateTime": "2019-04-25T23:45:40.42Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
