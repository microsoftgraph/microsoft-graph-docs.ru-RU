---
title: Тип перечисления managementAgentType
description: Тип агента управления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1711ad647afabc2b8877bd2f99b049bd1c1dd4e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914285"
---
# <a name="managementagenttype-enum-type"></a>Тип перечисления managementAgentType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
|microsoft365ManagedMdm|258|Это устройство управляется Microsoft 365 через Intune.|





