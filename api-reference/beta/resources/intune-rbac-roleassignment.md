---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 65a37c749380ce62da56f27aa335e89aa43b6e2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527550"
---
# <a name="roleassignment-resource-type"></a>Тип ресурса roleAssignment

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов roleAssignment](../api/intune-rbac-roleassignment-list.md)|Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)|Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Получение объекта roleAssignment](../api/intune-rbac-roleassignment-get.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md);|Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Создание объекта roleAssignment](../api/intune-rbac-roleassignment-create.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md);|Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Удаление объекта roleAssignment](../api/intune-rbac-roleassignment-delete.md)|Нет|Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).|
|[Обновление объекта roleAssignment](../api/intune-rbac-roleassignment-update.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|Строка|Отображаемое или понятное имя назначения роли.|
|description|String|Описание назначения роли.|
|скопемемберс|Коллекция String|Список идентификаторов групп безопасности с элементами области применения ролей.  Эти идентификаторы берутся из Azure Active Directory.|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);|Задает тип области для назначения роли. Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес. Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым. Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|
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



