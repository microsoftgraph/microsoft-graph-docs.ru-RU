---
title: Тип ресурса Девицеманажементусерригхтссеттинг
description: Представляет параметр прав пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14f17945232642df68e02a03ff0e1ec54ee5e220
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199371"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a>Тип ресурса Девицеманажементусерригхтссеттинг

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет параметр прав пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|[статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Представляет текущее состояние этого параметра прав пользователя. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|локалусерсорграупс|Коллекция [девицеманажементусерригхтслокалусерорграуп](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)|Представляет коллекцию локальных пользователей или групп, которые будут установлены на устройстве, если состояние этого параметра — разрешено. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```




