---
title: тип ресурса deviceManagementBooleanSettingInstance
description: Экземпляр параметра, представляющий значение boolean
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f2ccd2c88c5ef641ab8fc909f8aa625fafd6beb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134992"
---
# <a name="devicemanagementbooleansettinginstance-resource-type"></a>тип ресурса deviceManagementBooleanSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий значение boolean


Наследует [от deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementBooleanSettingInstances](../api/intune-deviceintent-devicemanagementbooleansettinginstance-list.md)|[коллекция deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Список свойств и связей [объектов deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|
|[Get deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-get.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Чтение свойств и связей [объекта deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|
|[Создание deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-create.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Создание нового [объекта deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|
|[Удаление deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-delete.md)|Нет|Удаляет [устройствоManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).|
|[Обновление deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-update.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Обновление свойств объекта [deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|String|ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|Boolean|Значение boolean|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementBooleanSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": true
}
```



