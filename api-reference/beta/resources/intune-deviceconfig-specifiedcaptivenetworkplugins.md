---
title: Тип ресурса СпеЦифиедкаптивенетворкплугинс
description: Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d205218aab1ef6fb5a59280ff25f5a22fde8c0b
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636319"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a>Тип ресурса СпеЦифиедкаптивенетворкплугинс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедбундлеидентифиерс|Коллекция String|Адрес сервера IKEv2. Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.specifiedCaptiveNetworkPlugins",
  "allowedBundleIdentifiers": [
    "String"
  ]
}
```



