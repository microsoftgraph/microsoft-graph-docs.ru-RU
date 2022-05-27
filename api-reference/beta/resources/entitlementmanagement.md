---
title: Тип ресурса entitlementManagement
description: Контейнер для ресурсов управления правами.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2768db11986466e864884d611877cf93dab6ef1a
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694899"
---
# <a name="entitlementmanagement-resource-type"></a>Тип ресурса entitlementManagement

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Одноэлементный элемент управления правами — это контейнер для ресурсов управления правами, включая [accessPackageCatalog](accesspackagecatalog.md), [connectedOrganization](connectedorganization.md) и [entitlementManagementSettings](entitlementmanagementsettings.md).  Полный список ресурсов см. в [обзоре управления правами](entitlementmanagement-overview.md).

Наследует [от сущности](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackageAssignmentPolicies|[Коллекция accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)| Представляет политику, которая определяет, какие субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета доступа. |
|accessPackageAssignmentRequests|[Коллекция accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Представляет запросы на назначение пакетов для доступа, созданные пользователем или от его имени.|
|accessPackageAssignmentResourceRoles|[Коллекция accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)| Представляет роль конкретного ресурса, назначенную субъекту с помощью назначения пакета доступа.|
|accessPackageAssignments|[Коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Назначение пакета доступа субъекту в течение определенного периода времени.|
|accessPackageCatalogs|[Коллекция accessPackageCatalog](../resources/accesspackagecatalog.md)|Контейнер пакетов доступа.|
|accessPackageResourceEnvironments|[Коллекция accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)| Ссылка на среду географического расположения, в которой находится ресурс.|
|accessPackageResourceRequests|[Коллекция accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Представляет запрос на добавление или удаление ресурса в каталог или из каталога соответственно. |
|accessPackageResourceRoleScopes|[Коллекция accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)| Ссылка как на область в ресурсе, так и на роль в этом ресурсе для этой области. |
|accessPackageResources|[Коллекция accessPackageResource](../resources/accesspackageresource.md)| Ссылка на ресурс, связанный с каталогом пакетов для доступа.|
|accessPackages|[Коллекция accessPackage](../resources/accesspackage.md)|Представляет объекты пакета доступа.|
|connectedOrganizations|[коллекция connectedOrganization](../resources/connectedorganization.md)|Представляет ссылки на каталог или домен другой организации, пользователи которой могут запрашивать доступ.|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Представляет параметры, которые могут управлять поведением Azure AD управления правами.|

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

