---
title: Тип перечисления managementAgentType
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 66441a37b417cef13cbb09219a26a98250cbf610
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888489"
---
# <a name="managementagenttype-enum-type"></a>Тип перечисления managementAgentType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Тип агента управления.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|EAS|1|Устройство управляется сервером Exchange server.|
|MDM|2|Устройство является управляемым путем MDM. Intune|
|easMdm|3|Устройство управляется сервером Exchange server и Intune MDM.|
|intuneClient|4|Управляемые клиентами Intune.|
|easIntuneClient|5|Устройство является EAS и Intune двойной управляемые клиентами.|
|configurationManagerClient|8|Устройство является управляемым, диспетчер конфигураций.|
|configurationManagerClientMdm|10|Устройство управляется Configuration Manager и MDM.|
|configurationManagerClientMdmEas|11|Устройство является управляемым, диспетчер конфигураций, MDM и Eas.|
|unknown|16|Тип агента управления UNKNOWN.|
|jamf|32|Атрибуты устройства полученные от Jamf.|
|googleCloudDevicePolicyController|64|Устройство управляется CloudDPC компании Google.|



