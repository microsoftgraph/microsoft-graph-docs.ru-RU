---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0afe1b3bbc06d634759e98aa6f04765177fb2126
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806924"
---
# <a name="roleassignment-resource-type"></a>Тип ресурса roleAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов roleAssignment](../api/intune-rbac-roleassignment-list.md)|Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)|Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Получение объекта roleAssignment](../api/intune-rbac-roleassignment-get.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Создание объекта roleAssignment](../api/intune-rbac-roleassignment-create.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Удаление объекта roleAssignment](../api/intune-rbac-roleassignment-delete.md)|Нет|Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Обновление объекта roleAssignment](../api/intune-rbac-roleassignment-update.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|Строка|Отображаемое или понятное имя назначения роли.|
|description|Строка|Описание назначения роли.|
|scopeMembers|Коллекция String|Список идентификаторов групп безопасности с элементами области применения ролей.  Эти идентификаторы берутся из Azure Active Directory.|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);|Указывает тип области назначения ролей. По умолчанию тип "ResourceScope" позволяет назначение ResourceScopes. Для "AllDevices", "AllLicensedUsers" и "AllDevicesAndLicensedUsers" свойство ResourceScopes следует оставить пустым. Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|
|resourceScopes|Коллекция String|Список идентификаторов групп безопасности с элементами области применения ролей.  Эти идентификаторы берутся из Azure Active Directory.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Определение роли, частью которого является это назначение.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```



