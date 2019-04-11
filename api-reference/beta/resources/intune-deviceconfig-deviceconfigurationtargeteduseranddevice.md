---
title: Тип ресурса Девицеконфигуратионтаржетедусеранддевице
description: Сводка по конфликтам для набора политик конфигурации устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2ddd31671f8cd277dbc7390c8c561189b6c0e3f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773002"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>Тип ресурса Девицеконфигуратионтаржетедусеранддевице

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по конфликтам для набора политик конфигурации устройств.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceId|String|Идентификатор устройства в возврате.|
|deviceName|String|Имя устройства в возврате.|
|userId|String|Идентификатор пользователя в возврате.|
|userDisplayName|String|Отображаемое имя пользователя в репозитории|
|userPrincipalName|String|ИМЯ участника-пользователя в возврате.|
|Ластчеккиндатетиме|DateTimeOffset|Время последнего возврата для этой связи пользователя и устройства.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





