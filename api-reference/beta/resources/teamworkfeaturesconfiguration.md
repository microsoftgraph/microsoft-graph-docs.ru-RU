---
title: тип ресурса teamworkFeaturesConfiguration
description: Представляет сведения Microsoft Teams конфигурации клиента для устройства с Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbd95b2fa6a5c20126712abb63eaf00f8c065823
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262710"
---
# <a name="teamworkfeaturesconfiguration-resource-type"></a>тип ресурса teamworkFeaturesConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения Microsoft Teams конфигурации клиента для устройства с Teams [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|emailToSendLogsAndFeedback|String|Адрес электронной почты для отправки журналов и отзывов.|
|isAutoScreenShareEnabled|Логическое|`True` если автоматический общий экран включен.|
|isBluetoothBeaconingEnabled|Логическое|`True`если Bluetooth включено маячок.|
|isHideMeetingNamesEnabled|Логическое|`True` если включено сокрытие имен собраний.|
|isSendLogsAndFeedbackEnabled|Логическое|`True` если включена отправка журналов и отзывов.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkFeaturesConfiguration",
  "emailToSendLogsAndFeedback": "String",
  "isAutoScreenShareEnabled": "Boolean",
  "isBluetoothBeaconingEnabled": "Boolean",
  "isHideMeetingNamesEnabled": "Boolean",
  "isSendLogsAndFeedbackEnabled": "Boolean"
}
```

