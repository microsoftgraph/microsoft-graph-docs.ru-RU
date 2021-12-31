---
title: тип ресурса accessPackageAssignment
description: Назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b394efdd7ac2cbc97ff1245af4e0d01d4392e3f4
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650624"
---
# <a name="accesspackageassignment-resource-type"></a>тип ресурса accessPackageAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-overview.md)назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.  Например, в назначении пакета доступа может быть установлено, что пользователю Алисе назначен доступ через пакет продаж пакета доступа за период с января 2019 г. по июль 2019 г.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Списки accessPackageAssignments](../api/entitlementmanagement-list-accesspackageassignments.md) | [коллекция accessPackageAssignment](accesspackageassignment.md) | Извлечение списка **объектов accessPackageAssignment.** |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Извлечение списка **объектов accessPackageAssignment,** фильтруемых на входе пользователя.|
| [reprocess](../api/accesspackageassignment-reprocess.md) | Нет | Автоматически переоплаты и принудительного выполнения назначений пользователя для определенного пакета доступа.|

> [!NOTE]
> Чтобы создать или удалить назначение пакета доступа для пользователя, используйте [создание accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageId|Строка|Идентификатор пакета доступа. Только для чтения.|
|assignmentPolicyId|Строка|Идентификатор политики назначения пакета доступа. Только для чтения.|
|assignmentState|Строка|Состояние назначения пакета доступа. Возможные значения `Delivering` , `Delivered` или `Expired` . Только для чтения. Поддерживает `$filter` (`eq`).|
|assignmentStatus|Строка|Дополнительные сведения о жизненном цикле назначения.  Возможные значения включают `Delivering` `Delivered` , или `NearExpiry1DayNotificationTriggered` `ExpiredNotificationTriggered` .  Только для чтения.|
|catalogId|Строка|Идентификатор каталога, содержащего пакет доступа. Только для чтения.|
|expiredDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения.|
|isExtended|Boolean|Указывает, расширено ли назначение пакета доступа. Только для чтения.|
|targetId|Строка| ID субъекта с назначением. Только для чтения.|
|schedule|[requestSchedule](requestschedule.md)| Когда назначение доступа должно быть на месте. Только для чтения.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Только для чтения. Допускается значение null. Поддерживает `$filter` `eq` () параметры **свойства id** `$expand` и запроса.|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Только для чтения. Допускается значение null. Поддерживает `$filter` `eq` () в **свойстве id**|
|accessPackageAssignmentResourceRoles|[коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)| Роли ресурсов, переданные целевому пользователю для этого назначения. Только для чтения. Допускается значение null.|
|target|[accessPackageSubject](accesspackagesubject.md)| Тема назначения пакета доступа. Только для чтения. Допускается значение null. Поддерживает `$expand`. Поддерживает `$filter` `eq` () на **objectId**. |

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
