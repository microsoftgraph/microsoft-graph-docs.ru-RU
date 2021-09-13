---
title: тип enum macOSContentCachingPeerPolicy
description: Определяет, с какой кэшей контента будут вглядывался другие кэши контента.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 89ad8ff2865e31b7d1ef1789093fe123e44f2e14
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017494"
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



