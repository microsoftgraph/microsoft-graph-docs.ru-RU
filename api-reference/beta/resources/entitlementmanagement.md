---
title: тип ресурса entitlementManagement
description: Контейнер для ресурсов управления правами.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c9c34a3699402f8d49fb2c0a0d9af3d5159a0eb3
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651831"
---
# <a name="entitlementmanagement-resource-type"></a>тип ресурса entitlementManagement

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Синглтон управления правами — это контейнер для ресурсов управления правами, включая [accessPackageCatalog,](accesspackagecatalog.md) [connectedOrganization](connectedorganization.md)и [entitlementManagementSettings.](entitlementmanagementsettings.md)  Полный список ресурсов см. в [обзоре управления правами.](entitlementmanagement-overview.md)

Наследует от [объекта](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection| Представляет политику, регулящую, какие субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа. |
|accessPackageAssignmentRequests|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Представляет запросы на назначение пакетов доступа, созданные пользователем или от имени пользователя.|
|accessPackageAssignmentResourceRoles|[коллекция accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)| Представляет определенную для ресурса роль, назначенную субъекту с помощью назначения пакета доступа.|
|accessPackageAssignments|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Представляет предоставление пакета доступа субъекту (пользователю или группе).|
|accessPackageCatalogs|[коллекция accessPackageCatalog](../resources/accesspackagecatalog.md)|Представляет группу пакетов доступа.|
|accessPackageResourceEnvironments|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection| Ссылка на среду геолокации, в которой находится ресурс.|
|accessPackageResourceRequests|[коллекция accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Представляет запрос на добавление или удаление ресурса в каталог или из него соответственно. |
|accessPackageResourceRoleScopes|[коллекция accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)| Ссылка как на область в ресурсе, так и на роль в этом ресурсе для этой области. |
|accessPackageResources|[коллекция accessPackageResource](../resources/accesspackageresource.md)| Ссылка на ресурс, связанный с каталогом пакетов доступа.|
|accessPackages|[коллекция accessPackage](../resources/accesspackage.md)|Представляет объекты пакета доступа.|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) collection|Представляет ссылки на каталог или домен другой организации, пользователи которой могут запрашивать доступ.|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Представляет параметры, которые контролируют поведение управления правами Azure AD.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagement",
  "id": "String (identifier)"
}
```

