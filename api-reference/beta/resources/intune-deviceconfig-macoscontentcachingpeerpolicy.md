---
title: тип enum macOSContentCachingPeerPolicy
description: Определяет, с какой кэшей контента будут вглядывался другие кэши контента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22adc6cd2df6dad85875deb190f40c305776a991
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783549"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a>тип enum macOSContentCachingPeerPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определяет, с какой кэшей контента будут вглядывался другие кэши контента.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|По умолчанию для одноранговых пользователей в локальной сети.|
|peersInLocalNetwork|1|Кэши контента будут одноранговых только с кэшами в их непосредственной локальной сети.|
|peersWithSamePublicIpAddress|2|Кэши контента будут одноранговых только с кэшами, которые имеют один и тот же общедоступный IP-адрес.|
|peersInCustomLocalNetworks|3|Кэши контента будут использовать contentCachingPeerFilterRanges и contentCachingPeerListenRanges, чтобы определить, с какой кэшой можно совмегать.|



