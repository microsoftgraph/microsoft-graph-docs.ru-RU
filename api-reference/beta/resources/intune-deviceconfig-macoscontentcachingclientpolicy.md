---
title: тип enum macOSContentCachingClientPolicy
description: Определяет, какие клиенты будут обслуживать кэш контента.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8bc8ab9be74dc9686ea534ae98ea170b4ed6760d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017501"
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
|clientsInLocalNetwork|1|Кэши контента будут предоставлять контент устройствам только в непосредственной локальной сети.|
|clientsWithSamePublicIpAddress|2|Кэши контента будут предоставлять контент устройствам с одинаковым общедоступным IP-адресом.|
|clientsInCustomLocalNetworks|3|Кэши контента будут предоставлять контент устройствам в contentCachingClientListenRanges.|
|customersInCustomLocalNetworksWithFallback|4 |Кэши контента будут предоставлять контент устройствам в contentCachingClientListenRanges, contentCachingPeerListenRanges и contentCachingParents.|



