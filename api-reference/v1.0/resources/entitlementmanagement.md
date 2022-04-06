---
title: тип ресурса entitlementManagement
description: Контейнер для ресурсов управления правами.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 33d5ef28494441d0bbc83d276ce74da6f9e49f8b
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608109"
---
# <a name="entitlementmanagement-resource-type"></a>тип ресурса entitlementManagement

Синглтон управления правами — это контейнер для ресурсов управления правами, включая [accessPackageCatalog](accesspackagecatalog.md), [connectedOrganization](connectedorganization.md) и [entitlementManagementSettings](entitlementmanagementsettings.md).  Полный список ресурсов см. в [обзоре управления правами](entitlementmanagement-overview.md).

Наследует [от сущности](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Это значение указывает на то, что ресурс — это однотон. Только для чтения. Наследуется от [сущности](entity.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackageAssignmentApprovals|[коллекция утверждений](../resources/approval.md) | Этапы утверждения запросов на назначение.|
|accessPackages|[коллекция accessPackage](../resources/accesspackage.md)|Представляет объекты пакета доступа.|
|assignmentPolicies|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection|Доступ к политикам назначения пакетов.|
|assignmentRequests|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Представляет запросы на назначение пакетов доступа, созданные пользователем или от имени пользователя.|
|assignments|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)| Представляет предоставление пакета доступа субъекту (пользователю или группе).|
|каталоги|[коллекция accessPackageCatalog](../resources/accesspackagecatalog.md)| Представляет коллекцию пакетов доступа.|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) collection|Представляет ссылки на каталог или домен другой организации, пользователи которой могут запрашивать доступ.|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)| Представляет параметры, которые контролируют поведение управления правами Azure AD.|

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


