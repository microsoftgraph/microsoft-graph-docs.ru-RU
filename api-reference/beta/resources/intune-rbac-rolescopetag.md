---
title: Тип ресурса roleScopeTag
description: Тег области ролей
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31f0bcb6abc187379f559f71fcaa1b7d96ce8a94
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337534"
---
# <a name="rolescopetag-resource-type"></a>Тип ресурса roleScopeTag

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тег области ролей

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List roleScopeTags](../api/intune-rbac-rolescopetag-list.md)|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Список свойств и связей объектов [roleScopeTag.](../resources/intune-rbac-rolescopetag.md)|
|[Get roleScopeTag](../api/intune-rbac-rolescopetag-get.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md);|Чтение свойств и связей объекта [roleScopeTag.](../resources/intune-rbac-rolescopetag.md)|
|[Создание roleScopeTag](../api/intune-rbac-rolescopetag-create.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md);|Создайте новый [объект roleScopeTag.](../resources/intune-rbac-rolescopetag.md)|
|[Удаление roleScopeTag](../api/intune-rbac-rolescopetag-delete.md)|Нет|Удаляет [рольScopeTag](../resources/intune-rbac-rolescopetag.md).|
|[Update roleScopeTag](../api/intune-rbac-rolescopetag-update.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md);|Обновление свойств объекта [roleScopeTag.](../resources/intune-rbac-rolescopetag.md)|
|[Действие assign](../api/intune-rbac-rolescopetag-assign.md)|[коллекция roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Пока не задокументировано.|
|[действие getRoleScopeTagsById](../api/intune-rbac-rolescopetag-getrolescopetagsbyid.md)|[Коллекция roleScopeTag](../resources/intune-rbac-rolescopetag.md)|Пока не задокументировано.|
|[функция hasCustomRoleScopeTag](../api/intune-rbac-rolescopetag-hascustomrolescopetag.md)|Boolean|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Это свойство доступно только для чтения и создается автоматически. Это свойство доступно только для чтения.|
|displayName|String|Отображение или дружеское имя тега Область ролей.|
|description|Строка|Описание тега Область ролей.|
|isBuiltIn|Boolean|Описание тега Область ролей. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|Список назначений для этого тега области ролей.|

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




