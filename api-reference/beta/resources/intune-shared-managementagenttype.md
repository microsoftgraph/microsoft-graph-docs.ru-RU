---
title: Тип перечисления managementAgentType
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a157111db947e9e7c186c30be6cc63a709b82922
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66672020"
---
# <a name="managementagenttype-enum-type"></a>Тип перечисления managementAgentType

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип агента управления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Eas|1|Устройство управляется сервером Exchange Server.|
|Mdm|2|Устройством управляет Intune MDM.|
|easMdm|3|Устройством управляет сервер Exchange Server и Intune MDM.|
|intuneClient|4|Intune управляемым клиентом.|
|easIntuneClient|5|Устройство является EAS и Intune управляемым двойным клиентом.|
|configurationManagerClient|8 |Устройством управляет Configuration Manager.|
|configurationManagerClientMdm|10|Устройством управляет Configuration Manager MDM.|
|ConfigurationManagerClientMdmEas|11|Устройством управляет Configuration Manager, MDM и Eas.|
|unknown|16|Неизвестный тип агента управления.|
|jamf|32|Атрибуты устройства извлекаются из Jamf.|
|googleCloudDevicePolicyController|64|Устройством управляет Google CloudDPC.|
|microsoft365ManagedMdm|258|Это устройство управляется Microsoft 365 через Intune.|
|msSense|1024|Пока не задокументировано.|
|intuneAosp|2048|Этим устройством управляет Intune MDM для устройств AOSP (Android Open Source Project).|




