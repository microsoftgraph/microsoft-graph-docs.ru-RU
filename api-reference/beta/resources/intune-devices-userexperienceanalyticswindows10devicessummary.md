---
title: тип ресурса userExperienceAnalyticsWindows10DevicesSummary
description: Аналитика пользовательских интерфейсов работает из любой Windows 10 устройств.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 101e764a1b5c6abd937d10a4b40642234a0f8dd3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046892"
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



