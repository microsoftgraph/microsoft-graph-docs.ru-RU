---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e09d73695c542c24fe6be297dec9496794d95fc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454285"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a>Тип ресурса Оффицеконфигуратионграупассигнменттаржет

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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



