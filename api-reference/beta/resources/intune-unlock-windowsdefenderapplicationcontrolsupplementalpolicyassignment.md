---
title: Тип ресурса Виндовсдефендераппликатионконтролсупплементалполициассигнмент
description: Класс, содержащий свойства, которые используются для назначения дополнительной политики Виндовсдефендераппликатионконтрол группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d340b8784ca59d4e0995ec8f370f9c35d7a4d3a6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729075"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicyassignment-resource-type"></a>Тип ресурса Виндовсдефендераппликатионконтролсупплементалполициассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для назначения дополнительной политики Виндовсдефендераппликатионконтрол группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсдефендераппликатионконтролсупплементалполициассигнментс](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-list.md)|Коллекция [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Список свойств и связей объектов [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .|
|[Получение Виндовсдефендераппликатионконтролсупплементалполициассигнмент](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-get.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Чтение свойств и связей объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .|
|[Создание Виндовсдефендераппликатионконтролсупплементалполициассигнмент](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-create.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .|
|[Удаление Виндовсдефендераппликатионконтролсупплементалполициассигнмент](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-delete.md)|Нет|Удаляет объект [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).|
|[Обновление Виндовсдефендераппликатионконтролсупплементалполициассигнмент](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment-update.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевое назначение группы, определенное администратором.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



