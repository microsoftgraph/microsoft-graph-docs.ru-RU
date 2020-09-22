---
title: Тип ресурса Ролескопетаг
description: Тег области применения роли
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4106ba2b3764621c94db52d92ca1d7b5e213dee0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039484"
---
# <a name="rolescopetag-resource-type"></a>Тип ресурса Ролескопетаг

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тег области применения роли

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|Коллекция [ролескопетаг](../resources/intune-rbac-rolescopetag.md)|Список свойств и связей объектов [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .|
|[Получение Ролескопетаг](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Чтение свойств и связей объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .|
|[Создание Ролескопетаг](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Создание нового объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .|
|[Удаление Ролескопетаг](../api/intune-rbac-rolescopetag-delete.md)|Нет|Удаляет объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md).|
|[Обновление Ролескопетаг](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Обновление свойств объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .|
|[Действие assign](../api/intune-rbac-rolescopetag-assign.md)|Коллекция [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md)|Пока не задокументировано.|
|[действие Жетролескопетагсбид](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|Коллекция [ролескопетаг](../resources/intune-rbac-rolescopetag.md)|Пока не задокументировано.|
|[Функция Хаскустомролескопетаг](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|Boolean|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|String|Отображаемое или понятное имя тега области применения роли.|
|description|String|Описание тега области применения роли.|
|isBuiltIn|Boolean|Описание тега области применения роли.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md)|Список назначений для тега области применения роли.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isBuiltIn": true
}
```






