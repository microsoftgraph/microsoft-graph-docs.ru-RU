---
title: Тип ресурса Девицеманажементусерригхтссеттинг
description: Представляет параметр прав пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b83e7c1c1c7409801b8ba79db2af6e4f167d0fd7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968467"
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






