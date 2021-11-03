---
title: тип ресурса windowsUpdateRolloutSettings
description: Сложный тип для хранения параметров обновления windows, включая время начала предложения, время конечной даты предложения и дни между каждым набором предложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d0d6849fcb41be6493f11a6d1b3d01c8409e9d6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688295"
---
# <a name="windowsupdaterolloutsettings-resource-type"></a>тип ресурса windowsUpdateRolloutSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения параметров обновления windows, включая время начала предложения, время конечной даты предложения и дни между каждым набором предложений.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|offerStartDateTimeInUTC|DateTimeOffset|Дата и время начала обновления функций, которые необходимо установить, обновить и отобразить для профиля обновления функций, например: 2020-06-09T10:00:00Z.|
|offerEndDateTimeInUTC|DateTimeOffset|Окончание даты и времени выпуска, обновления и отображения обновления функций, например: 2020-06-09T10:00:00Z.|
|offerIntervalInDays|Int32|Число дней между каждым набором предложений, которые будут заданы, обновлены и отображаются для профиля обновления функций, например: если OfferStartDateTimeInUTC 2020-06-09T10:00:00Z и OfferIntervalInDays — 1, Затем следующие два набора предложений будут последовательно делаться в 2020-06-10T10:00:00Z (на следующий день в указанное время) и 2020-06-11T10:00:00Z (на следующий день в указанное время) с 1 днем между каждым набором предложений.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateRolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateRolloutSettings",
  "offerStartDateTimeInUTC": "String (timestamp)",
  "offerEndDateTimeInUTC": "String (timestamp)",
  "offerIntervalInDays": 1024
}
```



