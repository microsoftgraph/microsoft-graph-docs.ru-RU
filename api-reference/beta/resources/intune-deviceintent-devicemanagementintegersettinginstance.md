---
title: тип ресурса deviceManagementIntegerSettingInstance
description: Экземпляр параметра, представляющий значение integer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 00bc87aad98ee687212268be76541dc08f1c74d0
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58798401"
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
|id|Строка|ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|Строка|ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|Строка|Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
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



