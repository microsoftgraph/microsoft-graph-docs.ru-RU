---
title: Тип ресурса androidDeviceOwnerUserFacingMessage
description: Представляет сообщение с пользователем с информацией о языковом стандарте, а также сообщение по умолчанию, которое будет использоваться, если языковой стандарт пользователя не соответствует ни одному из локализованных сообщений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07e57975a7aadf6e0d0dfe0b7479b66ef0c01d47
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213586"
---
# <a name="androiddeviceowneruserfacingmessage-resource-type"></a>Тип ресурса androidDeviceOwnerUserFacingMessage

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сообщение с пользователем с информацией о языковом стандарте, а также сообщение по умолчанию, которое будет использоваться, если языковой стандарт пользователя не соответствует ни одному из локализованных сообщений.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|localizedMessages|Коллекция [keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md)|Список <языкового стандарта и> сообщений. Эта коллекция может содержать не более 500 элементов.|
|defaultMessage|Строка|Сообщение по умолчанию, отображаемое, если языковой стандарт пользователя не соответствует ни одному из локализованных сообщений.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerUserFacingMessage",
  "localizedMessages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "defaultMessage": "String"
}
```




