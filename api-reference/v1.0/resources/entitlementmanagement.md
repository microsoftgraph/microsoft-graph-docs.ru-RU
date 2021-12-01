---
title: тип ресурса entitlementManagement
description: Singleton для совместимых ресурсов управления правами.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: db9b09efeea88ee3fc1d1dcfefab8d1ddb1c789e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242674"
---
# <a name="entitlementmanagement-resource-type"></a>тип ресурса entitlementManagement

Синглтон управления правами — это контейнер для ресурсов управления правами, включая [accessPackageCatalog,](accesspackagecatalog.md) [connectedOrganization](connectedorganization.md)и [entitlementManagementSettings.](entitlementmanagementsettings.md)  Полный список ресурсов см. в [обзоре управления правами.](entitlementmanagement-root.md)

Наследует от [объекта](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Это значение указывает на то, что ресурс — это однотон. Только для чтения. Наследуется от [сущности](entity.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackages|[коллекция accessPackage](../resources/accesspackage.md)|Пакеты доступа.|
|assignmentRequests|[accessPackageAssignmentRequest collection](../resources/accesspackageassignmentrequest.md)|Доступ к запросам на назначение пакета.|
|assignments|[коллекция accessPackageAssignment](../resources/accesspackageassignment.md)|Доступ к назначениям пакета.|
|каталоги|[коллекция accessPackageCatalog](../resources/accesspackagecatalog.md)|Доступ к каталогам пакетов.|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) collection|Подключенные организации.|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Параметры управления правами.|

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


