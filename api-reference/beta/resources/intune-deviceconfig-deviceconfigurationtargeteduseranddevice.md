---
title: тип ресурса deviceConfigurationTargetedUserAndDevice
description: Сводка конфликтов для набора политик конфигурации устройств.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84657d0401025473cc2f5628672eb413d3ac7ba4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051400"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>тип ресурса deviceConfigurationTargetedUserAndDevice

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка конфликтов для набора политик конфигурации устройств.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceId|String|Id устройства в проверке.|
|deviceName|String|Имя устройства в проверке.|
|userId|String|ID пользователя в проверке.|
|userDisplayName|String|Отображаемая фамилия пользователя в чеке|
|userPrincipalName|String|UpN пользователя в проверке.|
|lastCheckinDateTime|DateTimeOffset|Последнее время проверки для этой пары пользователей и устройств.|

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



