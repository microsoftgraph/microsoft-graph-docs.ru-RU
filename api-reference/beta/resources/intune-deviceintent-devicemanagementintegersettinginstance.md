---
title: тип ресурса deviceManagementIntegerSettingInstance
description: Экземпляр параметра, представляющий значение integer
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1bb7854ab3ce48376e611efacb6b10cb07adb857
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148160"
---
# <a name="devicemanagementintegersettinginstance-resource-type"></a>тип ресурса deviceManagementIntegerSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий значение integer


Наследует [от deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementIntegerSettingInstances](../api/intune-deviceintent-devicemanagementintegersettinginstance-list.md)|[коллекция deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|Список свойств и связей [объектов deviceManagementIntegerSettingInstance.](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|
|[Get deviceManagementIntegerSettingInstance](../api/intune-deviceintent-devicemanagementintegersettinginstance-get.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|Чтение свойств и связей [объекта deviceManagementIntegerSettingInstance.](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|
|[Создание deviceManagementIntegerSettingInstance](../api/intune-deviceintent-devicemanagementintegersettinginstance-create.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|Создание нового [объекта deviceManagementIntegerSettingInstance.](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|
|[Удаление deviceManagementIntegerSettingInstance](../api/intune-deviceintent-devicemanagementintegersettinginstance-delete.md)|Нет|Удаляет [устройствоManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).|
|[Обновление deviceManagementIntegerSettingInstance](../api/intune-deviceintent-devicemanagementintegersettinginstance-update.md)|[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|Обновление свойств объекта [deviceManagementIntegerSettingInstance.](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|String|ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|Int32|Значение integer|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntegerSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": 1024
}
```



