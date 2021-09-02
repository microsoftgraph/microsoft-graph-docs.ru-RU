---
title: тип ресурса userExperienceAnalyticsWindows10DevicesSummary
description: Аналитика пользовательских интерфейсов работает из любой Windows 10 устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: beeded0dfecec5f8c596e22a20c2352679a9fadc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797495"
---
# <a name="userexperienceanalyticswindows10devicessummary-resource-type"></a>тип ресурса userExperienceAnalyticsWindows10DevicesSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Аналитика пользовательских интерфейсов работает из любой Windows 10 устройств.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|unsupportedOSversionDeviceCount|Int32|Количество устройств Windows 10 с неподтверченными версиями ОС.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
  "unsupportedOSversionDeviceCount": 1024
}
```



