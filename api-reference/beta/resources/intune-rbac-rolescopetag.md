---
title: Тип ресурса roleScopeTag
description: Тег области роли
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3a63ac05ea6161843aa1ad664a99003b7f69d38e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400566"
---
# <a name="rolescopetag-resource-type"></a>Тип ресурса roleScopeTag

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тег области роли

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) коллекции|Свойства списка и связей объектов [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Получение roleScopeTag](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Чтение свойства и связи объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Создание roleScopeTag](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Создание нового объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|
|[Удаление roleScopeTag](../api/intune-rbac-rolescopetag-delete.md)|Нет|Удаляет [roleScopeTag](../resources/intune-rbac-rolescopetag.md).|
|[Обновление roleScopeTag](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Обновление свойства объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|String|Отображение или понятное имя тега область роли.|
|description|String|Описание тег область роли.|

## <a name="relationships"></a>Отношения
Нет

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




