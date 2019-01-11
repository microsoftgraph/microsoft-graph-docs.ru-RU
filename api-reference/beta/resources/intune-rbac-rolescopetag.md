---
title: Тип ресурса roleScopeTag
description: Тег области роли
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a48f74b9ecdb7a5f6eec87581fb0826160c4334b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830067"
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
|id|Строка|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|Строка|Отображение или понятное имя тега область роли.|
|описание|Строка|Описание тег область роли.|

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





