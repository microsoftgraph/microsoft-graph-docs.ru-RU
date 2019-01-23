---
title: Тип ресурса officeConfigurationGroupAssignmentTarget
description: Настройка клиента Office AAD группы конечного назначения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 411af117999498050288405874bd6b5baff5b6b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422749"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a>Тип ресурса officeConfigurationGroupAssignmentTarget

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка клиента Office AAD группы конечного назначения.

Наследуется от [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|groupId|String|Идентификатор группы AAD мы ориентация для настройки устройств.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



