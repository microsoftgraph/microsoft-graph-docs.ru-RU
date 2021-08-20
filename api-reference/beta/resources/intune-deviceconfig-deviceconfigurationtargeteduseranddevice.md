---
title: тип ресурса deviceConfigurationTargetedUserAndDevice
description: Сводка конфликтов для набора политик конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 671cbd9e5c6cf9448b86f8ce3f1bd852b794ca492e55b9c0edcbde8a01e0a3c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227479"
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




