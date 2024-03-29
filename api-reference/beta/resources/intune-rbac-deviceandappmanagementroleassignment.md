---
title: Тип ресурса deviceAndAppManagementRoleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f38cded5044e000ad0091ed65b1689fd966278e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030097"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a>Тип ресурса deviceAndAppManagementRoleAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к настраиваемым, так и ко встроенным ролям.


Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|Коллекция объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|
|[Получение объекта deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|
|[Создание объекта deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|
|[Удаление объекта deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|Нет|Удаление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|
|[Обновление объекта deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Это свойство доступно только для чтения и создается автоматически. Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|displayName|String|Отображаемое или понятное имя назначения роли. Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|description|String|Описание назначения роли. Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|scopeMembers|Коллекция String|Список идентификаторов групп безопасности с элементами области применения ролей.  Эти идентификаторы берутся из Azure Active Directory. Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);|Указывает тип области назначения ролей. По умолчанию тип "ResourceScope" позволяет назначение ResourceScopes. Для "AllDevices", "AllLicensedUsers" и "AllDevicesAndLicensedUsers" свойство ResourceScopes следует оставить пустым. Наследуется [от roleAssignment](../resources/intune-rbac-roleassignment.md). Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|
|resourceScopes|Коллекция String|Список идентификаторов групп безопасности с элементами области применения ролей.  Эти идентификаторы берутся из Azure Active Directory. Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|members|Коллекция String|Список идентификаторов групп безопасности с элементами ролей. Эти идентификаторы берутся из Azure Active Directory.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Определение роли, частью которого является это назначение. Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|roleScopeTags|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Набор тегов области ролей, определенных в назначении ролей.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



