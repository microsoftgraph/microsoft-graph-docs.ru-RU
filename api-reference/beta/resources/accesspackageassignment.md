---
title: тип ресурса accessPackageAssignment
description: Назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 866ac9f673bb3cf0ba7598dab2f3136b7b89a71b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265020"
---
# <a name="accesspackageassignment-resource-type"></a>тип ресурса accessPackageAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-root.md)назначение пакета доступа — это назначение пакета доступа определенному субъекту в течение определенного периода времени.  Например, в назначении пакета доступа может быть установлено, что пользователю Алисе назначен доступ через пакет продаж пакета доступа за период с января 2019 г. по июль 2019 г.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Списки accessPackageAssignments](../api/accesspackageassignment-list.md) | [коллекция accessPackageAssignment](accesspackageassignment.md) | Извлечение списка **объектов accessPackageAssignment.** |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Извлечение списка **объектов accessPackageAssignment,** фильтруемых на входе пользователя.|
| [reprocess](../api/accesspackageassignment-reprocess.md) | Нет | Автоматически переоплаты и принудительного выполнения назначений пользователя для определенного пакета доступа.|

>**Примечание:** Вы не можете использовать метод для создания или удаления назначения пакета доступа. Вместо этого клиент, который хочет запросить назначение пакета доступа для пользователя или удалить назначение пакета доступа у пользователя, может создать [accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageId|Строка|Идентификатор пакета доступа. Только для чтения.|
|assignmentPolicyId|Строка|Идентификатор политики назначения пакета доступа. Только для чтения.|
|assignmentState|Строка|Состояние назначения пакета доступа. Возможные значения `Delivering` , `Delivered` или `Expired` . Только для чтения.|
|assignmentStatus|Строка|Дополнительные сведения о жизненном цикле назначения.  Возможные значения включают `Delivering` `Delivered` , или `NearExpiry1DayNotificationTriggered` `ExpiredNotificationTriggered` .  Только для чтения.|
|catalogId|Строка|Идентификатор каталога, содержащего пакет доступа. Только для чтения.|
|expiredDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения.|
|isExtended|Логический|Указывает, расширено ли назначение пакета доступа. Только для чтения.|
|targetId|String| ID субъекта с назначением. Только для чтения.|
|schedule|[requestSchedule](requestschedule.md)| Когда назначение доступа должно быть на месте. Только для чтения.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Только для чтения. Допускается значение null.|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Только для чтения. Допускается значение null.|
|accessPackageAssignmentResourceRoles|[коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)| Роли ресурсов, переданные целевому пользователю для этого назначения. Только для чтения. Допускает значение null.|
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
