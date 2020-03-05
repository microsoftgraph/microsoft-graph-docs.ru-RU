---
title: Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг
description: Автонастройка глобального прокси-сервера владельца устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 207cbafb423b322fd954d561a4204150cb078abf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486600"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a>Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг

Пространство имен: Microsoft. Graph

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



