---
title: тип ресурса accessPackageAssignment
description: Назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e188857a2cc92210d9298d588c7d411e16fb688a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720286"
---
# <a name="accesspackageassignment-resource-type"></a>тип ресурса accessPackageAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-root.md)назначение пакета доступа — это назначение пакета доступа определенному субъекту на определенный период времени.  Например, в назначении пакета доступа может быть установлено, что пользователю Алисе назначен доступ через пакет продаж пакета доступа за период с января 2019 г. по июль 2019 г.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Списки accessPackageAssignments](../api/accesspackageassignment-list.md) | [коллекция accessPackageAssignment](accesspackageassignment.md) | Извлечение списка **объектов accesspackageassignment.** |

>**Примечание:** Вы не можете использовать метод для создания или удаления назначения пакета доступа. Вместо этого клиент, который хочет запросить назначение пакета доступа для пользователя или удалить назначение пакета доступа у пользователя, может создать [accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageId|String|Идентификатор пакета доступа. Только для чтения.|
|assignmentPolicyId|String|Идентификатор политики назначения пакета доступа. Только для чтения.|
|assignmentState|String|Состояние назначения пакета доступа. Возможные значения `Delivering` , `Delivered` или `Expired` . Только для чтения.|
|assignmentStatus|String|Дополнительные сведения о жизненном цикле назначения.  Возможные значения включают `Delivering` `Delivered` , или `NearExpiry1DayNotificationTriggered` `ExpiredNotificationTriggered` .  Только для чтения.|
|catalogId|String|Идентификатор каталога, содержащего пакет доступа. Только для чтения.|
|expiredDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения.|
|isExtended|Boolean|Указывает, расширено ли назначение пакета доступа. Только для чтения.|
|targetId|String| ID субъекта с назначением. Только для чтения.|
|schedule|[requestSchedule](requestschedule.md)| Когда назначение доступа должно быть на месте. Только для чтения.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Только для чтения. Допускается значение null.|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Только для чтения. Допускается значение null.|
|accessPackageAssignmentResourceRoles|[коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)| Роли ресурсов, переданные целевому пользователю для этого назначения. Только для чтения. Допускается значение null.|
|target|[accessPackageSubject](accesspackagesubject.md)| Тема назначения пакета доступа. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "keyProperty": "id"
}-->

```json
{
   "id":"9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
   "catalogId":"cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
   "accessPackageId":"e3f47362-993f-4fcb-8a38-532ffca16150",
   "assignmentPolicyId":"63ebd106-8116-40e7-a0ab-01ae475d11bb",
   "targetId":"ab4291f6-66b7-42bf-b597-a05b29414f5c",
   "assignmentStatus":"ExpiredNotificationTriggered",
   "assignmentState":"Expired",
   "isExtended":false,
   "expiredDateTime":"2019-04-25T23:45:40.42Z"
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


