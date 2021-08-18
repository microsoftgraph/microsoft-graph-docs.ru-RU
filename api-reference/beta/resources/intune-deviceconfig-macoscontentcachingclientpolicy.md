---
title: тип enum macOSContentCachingClientPolicy
description: Определяет, какие клиенты будут обслуживать кэш контента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 88030eec0996f0a5f2c80717a5b422495562a66e4e7133f0c3fc1665f1636855
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124733"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a>тип enum macOSContentCachingClientPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определяет, какие клиенты будут обслуживать кэш контента.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|По умолчанию для клиентов в локальной сети.|
|clientsInLocalNetwork|1 |Кэши контента будут предоставлять контент устройствам только в непосредственной локальной сети.|
|clientsWithSamePublicIpAddress|2|Кэши контента будут предоставлять контент устройствам с одинаковым общедоступным IP-адресом.|
|clientsInCustomLocalNetworks|3 |Кэши контента будут предоставлять контент устройствам в contentCachingClientListenRanges.|
|customersInCustomLocalNetworksWithFallback|4 |Кэши контента будут предоставлять контент устройствам в contentCachingClientListenRanges, contentCachingPeerListenRanges и contentCachingParents.|




