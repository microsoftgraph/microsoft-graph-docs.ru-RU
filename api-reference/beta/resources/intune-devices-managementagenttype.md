---
title: Тип перечисления managementAgentType
description: Тип агента управления.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401007"
---
# <a name="managementagenttype-enum-type"></a>Тип перечисления managementAgentType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|microsoft365ManagedMdm|258|Это устройство управляется Microsoft 365 через Intune.|




