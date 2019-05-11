---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 7458b1071b6133f3b46c8412270e30fdd0bf7638
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949313"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a>Тип ресурса Оффицеконфигуратионграупассигнменттаржет

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Целевой объект назначения группы AAD для группы клиентов Office.

Наследуется от [оффицеконфигуратионассигнменттаржет](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|groupId|String|Идентификатор группы AAD, на которую направляться конфигурация устройства.|

## <a name="relationships"></a>Связи
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



