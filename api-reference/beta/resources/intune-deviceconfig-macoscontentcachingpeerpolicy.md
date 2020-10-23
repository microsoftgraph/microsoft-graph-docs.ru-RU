---
title: тип перечисления Макосконтенткачингпирполици
description: Определяет, с каким содержимым будут кэшироваться другие кэши контента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1f55bd6aafffc7602632155e4fa3c387c888aae9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735815"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a><span data-ttu-id="c3a8e-103">тип перечисления Макосконтенткачингпирполици</span><span class="sxs-lookup"><span data-stu-id="c3a8e-103">macOSContentCachingPeerPolicy enum type</span></span>

<span data-ttu-id="c3a8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3a8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3a8e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3a8e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a8e-107">Определяет, с каким содержимым будут кэшироваться другие кэши контента.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-107">Determines which content caches other content caches will peer with.</span></span>

## <a name="members"></a><span data-ttu-id="c3a8e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c3a8e-108">Members</span></span>
|<span data-ttu-id="c3a8e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c3a8e-109">Member</span></span>|<span data-ttu-id="c3a8e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c3a8e-110">Value</span></span>|<span data-ttu-id="c3a8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3a8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a8e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c3a8e-112">notConfigured</span></span>|<span data-ttu-id="c3a8e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c3a8e-113">0</span></span>|<span data-ttu-id="c3a8e-114">По умолчанию используется значение Peer в локальной сети.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-114">Defaults to peers in local network.</span></span>|
|<span data-ttu-id="c3a8e-115">пирсинлокалнетворк</span><span class="sxs-lookup"><span data-stu-id="c3a8e-115">peersInLocalNetwork</span></span>|<span data-ttu-id="c3a8e-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c3a8e-116">1</span></span>|<span data-ttu-id="c3a8e-117">Кэш контента будет одноранговать только с кэшами в непосредственной локальной сети.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-117">Content caches will only peer with caches in their immediate local network.</span></span>|
|<span data-ttu-id="c3a8e-118">пирсвиссамепублиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="c3a8e-118">peersWithSamePublicIpAddress</span></span>|<span data-ttu-id="c3a8e-119">2</span><span class="sxs-lookup"><span data-stu-id="c3a8e-119">2</span></span>|<span data-ttu-id="c3a8e-120">Кэш контента будет иметь одноранговый узел с кэшами, которые используют один общий IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-120">Content caches will only peer with caches that share the same public IP address.</span></span>|
|<span data-ttu-id="c3a8e-121">пирсинкустомлокалнетворкс</span><span class="sxs-lookup"><span data-stu-id="c3a8e-121">peersInCustomLocalNetworks</span></span>|<span data-ttu-id="c3a8e-122">4</span><span class="sxs-lookup"><span data-stu-id="c3a8e-122">3</span></span>|<span data-ttu-id="c3a8e-123">Кэши контента будут использовать Контенткачингпирфилтерранжес и Контенткачингпирлистенранжес для определения кэшей, с которыми осуществляется одноранговая связь.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-123">Content caches will use contentCachingPeerFilterRanges and contentCachingPeerListenRanges to determine which caches to peer with.</span></span>|





