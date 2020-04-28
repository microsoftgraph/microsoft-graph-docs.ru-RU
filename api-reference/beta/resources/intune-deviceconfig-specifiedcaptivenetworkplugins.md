---
title: Тип ресурса СпеЦифиедкаптивенетворкплугинс
description: Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6752e045817e9a03eefae178d7df15d152f0ea58
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412771"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a>Тип ресурса СпеЦифиедкаптивенетворкплугинс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедбундлеидентифиерс|Коллекция объектов string|Адрес сервера IKEv2. Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN|

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



