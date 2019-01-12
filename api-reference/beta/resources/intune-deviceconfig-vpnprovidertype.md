---
title: Тип перечисления vpnProviderType
description: Тип поставщика для VPN-app.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1eeb0acf2f6e7b0773cbf4697e5a27699d1f2f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937728"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="7f6a9-103">Тип перечисления vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="7f6a9-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="7f6a9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f6a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f6a9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f6a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f6a9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f6a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f6a9-107">Тип поставщика для VPN-app.</span><span class="sxs-lookup"><span data-stu-id="7f6a9-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="7f6a9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7f6a9-108">Members</span></span>
|<span data-ttu-id="7f6a9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7f6a9-109">Member</span></span>|<span data-ttu-id="7f6a9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7f6a9-110">Value</span></span>|<span data-ttu-id="7f6a9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7f6a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f6a9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7f6a9-112">notConfigured</span></span>|<span data-ttu-id="7f6a9-113">0</span><span class="sxs-lookup"><span data-stu-id="7f6a9-113">0</span></span>|<span data-ttu-id="7f6a9-114">Туннель трафика явно не настроен.</span><span class="sxs-lookup"><span data-stu-id="7f6a9-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="7f6a9-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="7f6a9-115">appProxy</span></span>|<span data-ttu-id="7f6a9-116">1</span><span class="sxs-lookup"><span data-stu-id="7f6a9-116">1</span></span>|<span data-ttu-id="7f6a9-117">Туннель трафика на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="7f6a9-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="7f6a9-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="7f6a9-118">packetTunnel</span></span>|<span data-ttu-id="7f6a9-119">2</span><span class="sxs-lookup"><span data-stu-id="7f6a9-119">2</span></span>|<span data-ttu-id="7f6a9-120">Туннель трафика на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="7f6a9-120">Tunnel traffic at the IP layer.</span></span>|





