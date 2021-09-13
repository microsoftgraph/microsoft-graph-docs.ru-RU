---
title: тип ресурса mobileAppInstallTimeSettings
description: Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eeff26a918e12ce0b08685f8c64385ea77e6873c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062672"
---
# <a name="mobileappinstalltimesettings-resource-type"></a>тип ресурса mobileAppInstallTimeSettings

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для определения того, когда предлагать приложение устройствам и когда устанавливать приложение на устройствах.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|useLocalTime|Логический|Следует ли использовать местное время устройства или время UTC при определении доступных и крайних сроков.|
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




