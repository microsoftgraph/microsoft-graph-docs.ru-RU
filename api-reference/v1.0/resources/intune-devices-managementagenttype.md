---
title: тип enum managementAgentType
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fc6669fae134a53886a425fab2635f9ef83d7c4626fcb1056a0d7cda179d932b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149858"
---
# <a name="managementagenttype-enum-type"></a>тип enum managementAgentType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип агента управления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|eas|1|Устройство управляется Exchange сервером.|
|mdm|2|Устройство управляется intune MDM.|
|easMdm|3|Устройство управляется как сервером Exchange, так и MDM Intune.|
|intuneClient|4 |Клиент Intune управляется.|
|easIntuneClient|5 |Устройство является двойным управляемым клиентом EAS и Intune.|
|configurationManagerClient|8 |Устройство управляется диспетчером конфигурации.|
|configurationManagerClientMdm|10 |Устройство управляется диспетчером конфигурации и MDM.|
|configurationManagerClientMdmEas|11|Устройство управляется диспетчером конфигурации, MDM и Eas.|
|unknown|16 |Неизвестный тип агента управления.|
|jamf|32|Атрибуты устройства извлекаются из Jamf.|
|googleCloudDevicePolicyController|64|Устройство управляется cloudDPC От Google.|




