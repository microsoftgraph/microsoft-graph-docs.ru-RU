---
title: тип ресурса mobileAppInstallTimeSettings
description: Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bb768938ffa2e167f13a267451041b65f39011c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755121"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>тип ресурса mobileAppInstallTimeSettings

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|useLocalTime|Boolean|Следует ли использовать местное время устройства или время UTC при определении доступных и крайних сроков.|
|startDateTime|DateTimeOffset|Время, в которое приложение должно быть доступно для установки.|
|deadlineDateTime|DateTimeOffset|Время установки приложения.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```




