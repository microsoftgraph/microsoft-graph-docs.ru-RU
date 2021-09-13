---
title: тип ресурса deviceManagementStringSettingInstance
description: Экземпляр параметра, представляющий значение строки
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 95600e68afbfb8729770a08cebbc68273e24a82d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086400"
---
# <a name="devicemanagementstringsettinginstance-resource-type"></a>тип ресурса deviceManagementStringSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий значение строки


Наследует [от deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementStringSettingInstances](../api/intune-deviceintent-devicemanagementstringsettinginstance-list.md)|[коллекция deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Список свойств и связей [объектов deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|
|[Get deviceManagementStringSettingInstance](../api/intune-deviceintent-devicemanagementstringsettinginstance-get.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Чтение свойств и связей [объекта deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|
|[Создание deviceManagementStringSettingInstance](../api/intune-deviceintent-devicemanagementstringsettinginstance-create.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Создание нового [объекта deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|
|[Удаление deviceManagementStringSettingInstance](../api/intune-deviceintent-devicemanagementstringsettinginstance-delete.md)|Нет|Удаляет [устройствоManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).|
|[Обновление deviceManagementStringSettingInstance](../api/intune-deviceintent-devicemanagementstringsettinginstance-update.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Обновление свойств объекта [deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|String|ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|String|Значение строки|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementStringSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": "String"
}
```



