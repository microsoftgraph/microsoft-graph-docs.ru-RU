---
title: Тип ресурса roleScopeTag
description: Тег области роли
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 609d4202069f6e4258c9824a65b72ab769c365b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981856"
---
# <a name="rolescopetag-resource-type"></a>Тип ресурса roleScopeTag

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|описание|String|Описание тег область роли.|

## <a name="relationships"></a>Связи
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





