---
title: тип ресурса deviceManagementComplexSettingInstance
description: Экземпляр параметра, представляющий сложное значение
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b3c8afeed7102f1267349dc72824a8cace6427f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802994"
---
# <a name="devicemanagementcomplexsettinginstance-resource-type"></a>тип ресурса deviceManagementComplexSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий сложное значение


Наследует [от deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementComplexSettingInstances](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-list.md)|[коллекция deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Список свойств и связей [объектов deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|
|[Get deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-get.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Чтение свойств и связей [объекта deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|
|[Создание deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-create.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Создание нового [объекта deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|
|[Удаление deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-delete.md)|Нет|Удаляет [устройствоManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).|
|[Обновление deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-update.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Обновление свойств объекта [deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|Строка|ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|Строка|Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|значение|[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Значения, которые составляют сложный параметр|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplexSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```



