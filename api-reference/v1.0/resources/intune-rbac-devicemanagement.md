---
title: Тип ресурса deviceManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4b06bb4f6f9fdc55540c8a2361acf4afd6eeffa420b30e424b7d67417613e53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235466"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-rbac-devicemanagement-get.md)|[deviceManagement](../resources/intune-rbac-devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-rbac-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-rbac-devicemanagement-update.md)|[deviceManagement](../resources/intune-rbac-devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune-rbac-devicemanagement.md).|
|[Функция getEffectivePermissions](../api/intune-rbac-devicemanagement-geteffectivepermissions.md)|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Получает действующие разрешения пользователя, прошедшего проверку подлинности|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleDefinitions|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Определения ролей.|
|roleAssignments|Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Назначения ролей.|
|resourceOperations|Коллекция [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Операции с ресурсами.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




