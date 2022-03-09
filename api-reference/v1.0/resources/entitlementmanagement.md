---
title: тип ресурса entitlementManagement
description: Контейнер для ресурсов управления правами.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 547e8140ecfb39686b028e967aaf1328f2f077a2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393131"
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
|assignmentRequests|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Представляет запросы на назначение пакетов доступа, созданные пользователем или от имени пользователя.|
|assignments|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)| Представляет предоставление пакета доступа субъекту (пользователю или группе).|
|каталоги|[коллекция accessPackageCatalog](../resources/accesspackagecatalog.md)| Представляет группу пакетов доступа.|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) collection|Представляет ссылки на каталог или домен другой организации, пользователи которой могут запрашивать доступ.|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)| Представляет параметры, которые контролируют поведение управления правами Azure AD.|

## <a name="json-representation"></a>Представление в формате JSON
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


