---
title: тип ресурса androidDeviceOwnerSystemUpdateFreezePeriod
description: Представляет один элемент в списке периодов замораживания для обновлений системы владельца устройств Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54c3d150a579f981eccbe03dfccddfaf8b02b701
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712231"
---
# <a name="androiddeviceownersystemupdatefreezeperiod-resource-type"></a>тип ресурса androidDeviceOwnerSystemUpdateFreezePeriod

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет один элемент в списке периодов замораживания для обновлений системы владельца устройств Android

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startMonth|Int32|Месяц даты начала периода замораживания. Допустимые значения от 1 до 12|
|startDay|Int32|День начала периода заморозки. Допустимые значения от 1 до 31|
|endMonth|Int32|Месяц окончания периода замораживания. Допустимые значения от 1 до 12|
|endDay|Int32|День окончания периода замораживания. Допустимые значения от 1 до 31|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
  "startMonth": 1024,
  "startDay": 1024,
  "endMonth": 1024,
  "endDay": 1024
}
```




