---
title: тип ресурса userExperienceAnalyticsWindows10DevicesSummary
description: Аналитика пользовательских интерфейсов работает из любого сводки устройств Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f43c2848902b6d9fbb3e54a2fd9a8ac36edc0793
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146830"
---
# <a name="userexperienceanalyticswindows10devicessummary-resource-type"></a>тип ресурса userExperienceAnalyticsWindows10DevicesSummary

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Аналитика пользовательских интерфейсов работает из любого сводки устройств Windows 10.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|unsupportedOSversionDeviceCount|Int32|Количество устройств с Windows 10 с неподтверченными версиями ОС.|

## <a name="relationships"></a>Отношения
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




