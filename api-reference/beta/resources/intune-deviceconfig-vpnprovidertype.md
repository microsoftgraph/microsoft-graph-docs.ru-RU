---
title: Тип перечисления vpnProviderType
description: Тип поставщика для VPN-app.
author: tfitzmac
ms.openlocfilehash: d8f002582879302bcbe0fb965110eaa5e674a689
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351599"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="343f2-103">Тип перечисления vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="343f2-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="343f2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="343f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="343f2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="343f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="343f2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="343f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="343f2-107">Тип поставщика для VPN-app.</span><span class="sxs-lookup"><span data-stu-id="343f2-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="343f2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="343f2-108">Members</span></span>
|<span data-ttu-id="343f2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="343f2-109">Member</span></span>|<span data-ttu-id="343f2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="343f2-110">Value</span></span>|<span data-ttu-id="343f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="343f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="343f2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="343f2-112">notConfigured</span></span>|<span data-ttu-id="343f2-113">0</span><span class="sxs-lookup"><span data-stu-id="343f2-113">0</span></span>|<span data-ttu-id="343f2-114">Туннель трафика явно не настроен.</span><span class="sxs-lookup"><span data-stu-id="343f2-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="343f2-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="343f2-115">appProxy</span></span>|<span data-ttu-id="343f2-116">1</span><span class="sxs-lookup"><span data-stu-id="343f2-116">1</span></span>|<span data-ttu-id="343f2-117">Туннель трафика на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="343f2-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="343f2-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="343f2-118">packetTunnel</span></span>|<span data-ttu-id="343f2-119">2</span><span class="sxs-lookup"><span data-stu-id="343f2-119">2</span></span>|<span data-ttu-id="343f2-120">Туннель трафика на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="343f2-120">Tunnel traffic at the IP layer.</span></span>|





