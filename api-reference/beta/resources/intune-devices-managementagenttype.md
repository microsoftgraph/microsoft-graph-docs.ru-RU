---
title: тип enum managementAgentType
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f1593d4f25a3da7f631c69e105dc8652453e01f6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58815045"
---
# <a name="managementagenttype-enum-type"></a>тип enum managementAgentType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|configurationManagerClientMdmEas|11 |Устройство управляется диспетчером конфигурации, MDM и Eas.|
|unknown|16 |Неизвестный тип агента управления.|
|jamf|32|Атрибуты устройства извлекаются из Jamf.|
|googleCloudDevicePolicyController|64|Устройство управляется cloudDPC От Google.|
|Microsoft365ManagedMdm|258|Это устройство управляется Microsoft 365 через Intune.|
|msSense|1024|Пока не задокументировано.|
|intuneAosp|2048|Это устройство управляется устройствами MDM intune для AOSP (Android Open Source Project)|



