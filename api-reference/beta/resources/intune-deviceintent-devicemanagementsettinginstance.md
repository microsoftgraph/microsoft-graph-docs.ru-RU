---
title: тип ресурса deviceManagementSettingInstance
description: Базовый тип для экземпляра параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffebf2d3c9fd5df67e705d80dd0fe412ba32f32b13ddff672cbdcd47a1b43442
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54179055"
---
# <a name="devicemanagementsettinginstance-resource-type"></a>тип ресурса deviceManagementSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый тип для экземпляра параметра

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementSettingInstances](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Список свойств и связей [объектов deviceManagementSettingInstance.](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|[Get deviceManagementSettingInstance](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Чтение свойств и связей [объекта deviceManagementSettingInstance.](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID экземпляра параметра|
|definitionId|Строка|ID определения параметра для этого экземпляра|
|valueJson|Строка|Представление значения JSON|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```




