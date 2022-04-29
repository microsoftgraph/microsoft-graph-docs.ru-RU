---
title: Тип ресурса accessPackageAssignment
description: Назначение пакета доступа — это назначение пакета доступа определенной теме на определенный период времени.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0c7ad4cd5ac58f2fea227a2fdb84cfc938797446
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133386"
---
# <a name="accesspackageassignment-resource-type"></a>Тип ресурса accessPackageAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD управления правами](entitlementmanagement-overview.md) назначение пакета доступа — это назначение пакета доступа определенной теме на определенный период времени.  Например, назначение пакета доступа может указать, что пользователю Алисе был назначен доступ через пакет доступа Sales за период с января 2019 г. по июль 2019 г.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление объектов accessPackageAssignment](../api/entitlementmanagement-list-accesspackageassignments.md) | [Коллекция accessPackageAssignment](accesspackageassignment.md) | Получение списка объектов **accessPackageAssignment** . |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Получение списка объектов **accessPackageAssignment** , отфильтрованных по пользователю, выполнившего вход.|
| [Повторная обработка](../api/accesspackageassignment-reprocess.md) | Нет | Автоматически переоценка и принудительное применение назначений пользователя для определенного пакета доступа.|
| [коллекция additionalAccess](../api/accesspackageassignment-additionalaccess.md) [accessPackageAssignment](../resources/accesspackageassignment.md)|Получение списка объектов **accessPackageAssignment** для пользователей, имеющих назначения несовместимым пакетам доступа.|

> [!NOTE]
> Чтобы создать или удалить назначение пакета доступа для пользователя, используйте [команду accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageId|String|Идентификатор пакета доступа. Только для чтения.|
|assignmentPolicyId|String|Идентификатор политики назначения пакетов для доступа. Только для чтения.|
|assignmentState|String|Состояние назначения пакета доступа. Возможные значения: `Delivering`, `Delivered`или `Expired`. Только для чтения. Поддерживает `$filter` (`eq`).|
|assignmentStatus|String|Дополнительные сведения о жизненном цикле назначения.  Возможные значения: `Delivering`, `Delivered`или `NearExpiry1DayNotificationTriggered``ExpiredNotificationTriggered`.  Только для чтения.|
|catalogId|String|Идентификатор каталога, содержащего пакет доступа. Только для чтения.|
|expiredDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения.|
|isExtended|Логическое|Указывает, расширено ли назначение пакета доступа. Только для чтения.|
|targetId|String| Идентификатор субъекта с назначением. Только для чтения.|
|schedule|[requestSchedule](requestschedule.md)| Когда назначение доступа должно быть установлено. Только для чтения.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Только для чтения. Допускается значение null. `$filter` Поддерживает (`eq`) для **свойства идентификатора** и параметров `$expand` запроса.|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Только для чтения. Допускается значение null. `$filter` Поддерживает (`eq`) свойство **id**.|
|accessPackageAssignmentResourceRoles|[Коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)| Роли ресурсов, доставленные целевому пользователю для этого назначения. Только для чтения. Допускается значение null.|
|target|[accessPackageSubject](accesspackagesubject.md)| Тема назначения пакета доступа. Только для чтения. Допускается значение null. Поддерживает `$expand`. Поддерживает (`$filter``eq`) для **objectId**. |

## <a name="json-representation"></a>Представление в формате JSON

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
