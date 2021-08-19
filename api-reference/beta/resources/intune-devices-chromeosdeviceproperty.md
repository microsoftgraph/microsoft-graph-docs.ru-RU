---
title: тип ресурса chromeOSDeviceProperty
description: Представляет свойство устройства ChromeOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c2688b4b3459232af9f2948e3f1cdb2c7ac7fc20afeecacd209e3eb4e0df4374
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54232596"
---
# <a name="chromeosdeviceproperty-resource-type"></a>тип ресурса chromeOSDeviceProperty

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет свойство устройства ChromeOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя свойства|
|value|String|Значение свойства|
|valueType|Строка|Тип значения|
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




