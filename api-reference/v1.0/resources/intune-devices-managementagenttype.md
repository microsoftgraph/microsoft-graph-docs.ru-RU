---
title: Тип перечисления managementAgentType
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8e178c22a13e089b89b709757f38d9abb3cc04df
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731934"
---
# <a name="managementagenttype-enum-type"></a>Тип перечисления managementAgentType

Пространство имен: microsoft.graph

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





