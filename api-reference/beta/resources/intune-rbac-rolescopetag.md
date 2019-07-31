---
title: Тип ресурса Ролескопетаг
description: Тег области применения роли
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 805f130945f4e8b966c35409f6e27fcf55e3f02f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967597"
---
# <a name="rolescopetag-resource-type"></a>Тип ресурса Ролескопетаг

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|displayName|Строка|Отображаемое или понятное имя тега области применения роли.|
|description|String|Описание тега области применения роли.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
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
  "description": "String"
}
```





