---
title: Тип ресурса Акцесспаккажеассигнмент
description: Назначение пакета Access — это назначение пакета Access определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b52b9dbd7b2b76df34ab6c55a46b69718d4a0e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508564"
---
# <a name="accesspackageassignment-resource-type"></a>Тип ресурса Акцесспаккажеассигнмент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)назначение пакета Access — это назначение пакета доступа определенной теме в течение определенного периода времени.  Например, при назначении пакета доступа может быть задано, что пользователю "Алиса" назначен доступ через пакет Access "продажи" в течение периода с 2019 по 2019 июля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Акцесспаккажеассигнментс](../api/accesspackageassignment-list.md) | Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md) | Получение списка объектов **акцесспаккажеассигнмент** . |

>**Примечание:** Невозможно использовать метод для создания или удаления назначения пакета Access. Вместо этого клиент, которому требуется запрашивать назначение пакета доступа для пользователя или удалять назначение пакета Access пользователю, может [создать акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккажеид|String|Идентификатор пакета Access. Только для чтения.|
|ассигнментполициид|String|Идентификатор политики назначения пакетов доступа. Только для чтения.|
|ассигнментстате|String|Состояние пакета Access. Возможные значения: `Delivered` или `Expired`. Только для чтения.|
|Свойства assignmentstatus|String|Только для чтения.|
|каталогид|String|Идентификатор каталога, содержащего пакет Access. Только для чтения.|
|експиреддатетиме|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|Расширенная|Boolean|Указывает, является ли назначение пакета доступа расширенным. Только для чтения.|
|targetId|String| ИДЕНТИФИКАТОР субъекта с назначением. Только для чтения.|

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
