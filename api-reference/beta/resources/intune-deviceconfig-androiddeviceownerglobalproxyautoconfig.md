---
title: Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг
description: Автонастройка глобального прокси-сервера владельца устройств Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3cee579dbd5a8dee57b270e117a0c50aca377f94
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402987"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a>Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Автонастройка глобального прокси-сервера владельца устройств Android.


Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|проксяутоконфигурл|String|URL-адрес автоматической настройки прокси-сервера|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
  "proxyAutoConfigURL": "String"
}
```



