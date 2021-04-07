---
title: тип ресурса chromeOSDeviceProperty
description: Представляет свойство устройства ChromeOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42b4903965d90641955659277360c46428562ed4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612272"
---
# <a name="chromeosdeviceproperty-resource-type"></a>тип ресурса chromeOSDeviceProperty

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет свойство устройства ChromeOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя свойства|
|value|String|Значение свойства|
|valueType|String|Тип значения|
|updatable|Логический|Является ли это свойство updatable|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chromeOSDeviceProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSDeviceProperty",
  "name": "String",
  "value": "String",
  "valueType": "String",
  "updatable": true
}
```




