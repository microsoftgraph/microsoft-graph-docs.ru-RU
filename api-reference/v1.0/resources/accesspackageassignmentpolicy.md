---
title: тип ресурса accessPackageAssignmentPolicy
description: Политика назначения пакета доступа указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 90f2b6024e63325a1e0c7e6d8156fa40189736b9
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608401"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>тип ресурса accessPackageAssignmentPolicy

Пространство имен: microsoft.graph

В [управлении правами Azure AD](entitlementmanagement-overview.md) политика назначения пакетов доступа указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа. Пакет доступа может иметь нулевую или несколько политик. При получении запроса субъекта субъекту соответствует каждая политика, чтобы найти политику (если таково) с **requestorSettings** , которые включают этот субъект. Затем политика определяет, требует ли запрос утверждения, продолжительности назначения пакета доступа и требует ли назначение регулярных отзывов.

Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) , который ссылается на политику назначения пакета доступа и пакета доступа.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessPackageAssignmentPolicies](../api/entitlementmanagement-list-assignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection|Получите список объектов [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) и их свойств.|
|[Создание accessPackageAssignmentPolicy](../api/entitlementmanagement-post-assignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Создание нового [объекта accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Получить accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Обновление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Обновление свойств объекта [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Удаление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md)|Нет|Удаляет объект [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedTargetScope|allowedTargetScope|Директора, которые могут быть назначены пакету доступа с помощью этой политики. Возможные значения: `notSpecified`, `specificDirectoryUsers`, `specificConnectedOrganizationUsers`, `specificDirectoryServicePrincipals`, `allMemberUsers`, `allDirectoryUsers`, `allDirectoryServicePrincipals`, `allConfiguredConnectedOrganizationUsers`, `allExternalUsers`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|description|Строка|Описание политики.|
|displayName|Строка|Отображает имя политики.|
|истечение срока действия|[expirationPattern](../resources/expirationpattern.md)|Срок действия для назначений, созданных в этой политике.|
|id|Строка|Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|Указывает параметры для утверждения запросов на назначение пакета доступа с помощью этой политики. Например, если требуется утверждение для новых запросов.|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|Предоставляет дополнительные параметры, чтобы выбрать, кто может создать запрос на назначение пакета доступа с помощью этой политики и что они могут включить в свой запрос.|
|reviewSettings|[accessPackageAssignmentReviewSettings](../resources/accesspackageassignmentreviewsettings.md)|Параметры для проверки доступа к назначениям с помощью этой политики.|
|specificAllowedTargets|[коллекция subjectSet](../resources/subjectset.md)|Принципы, которые могут быть назначены доступ из пакета доступа через эту политику.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|Пакет доступа, содержащий эту политику. Только для чтения. |
|каталог|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Каталог пакета доступа, содержащего эту политику. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "allowedTargetScope": "String",
  "specificAllowedTargets": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "requestorSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentRequestorSettings"
  },
  "requestApprovalSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentApprovalSettings"
  },
  "reviewSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentReviewSettings"
  },
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


