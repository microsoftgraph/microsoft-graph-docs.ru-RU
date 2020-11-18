---
title: Тип ресурса Девицеконфигуратионтаржетедусеранддевице
description: Сводка по конфликтам для набора политик конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c722cf1a21e46ec6066efc1e836793d77ce8e8b7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199394"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>Тип ресурса Девицеконфигуратионтаржетедусеранддевице

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по конфликтам для набора политик конфигурации устройств.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceId|String|Идентификатор устройства в возврате.|
|deviceName|String|Имя устройства в возврате.|
|userId|String|Идентификатор пользователя в возврате.|
|userDisplayName|String|Отображаемое имя пользователя в репозитории|
|userPrincipalName|String|Имя участника-пользователя в возврате.|
|ластчеккиндатетиме|DateTimeOffset|Время последнего возврата для этой связи пользователя и устройства.|

## <a name="relationships"></a>Связи
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




