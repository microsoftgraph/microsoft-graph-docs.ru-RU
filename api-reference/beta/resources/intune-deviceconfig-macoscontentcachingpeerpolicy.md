---
title: тип enum macOSContentCachingPeerPolicy
description: Определяет, с какой кэшей контента будут вглядывался другие кэши контента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b89b7043ca64f106ec1d3bbded041ae15461195c916db0d31cf32dd848d42e40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54181197"
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
|peersInLocalNetwork|1 |Кэши контента будут одноранговых только с кэшами в их непосредственной локальной сети.|
|peersWithSamePublicIpAddress|2|Кэши контента будут одноранговых только с кэшами, которые имеют один и тот же общедоступный IP-адрес.|
|peersInCustomLocalNetworks|3 |Кэши контента будут использовать contentCachingPeerFilterRanges и contentCachingPeerListenRanges, чтобы определить, с какой кэшой можно совмегать.|




