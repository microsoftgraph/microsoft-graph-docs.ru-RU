---
title: Тип перечисления vpnProviderType
description: Тип поставщика для VPN-app.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2de8f78222ba0c945000b84f28039c2f6af58daa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407223"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="b8091-103">Тип перечисления vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="b8091-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="b8091-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b8091-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b8091-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8091-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8091-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8091-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8091-107">Тип поставщика для VPN-app.</span><span class="sxs-lookup"><span data-stu-id="b8091-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="b8091-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b8091-108">Members</span></span>
|<span data-ttu-id="b8091-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b8091-109">Member</span></span>|<span data-ttu-id="b8091-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b8091-110">Value</span></span>|<span data-ttu-id="b8091-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b8091-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8091-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b8091-112">notConfigured</span></span>|<span data-ttu-id="b8091-113">0</span><span class="sxs-lookup"><span data-stu-id="b8091-113">0</span></span>|<span data-ttu-id="b8091-114">Туннель трафика явно не настроен.</span><span class="sxs-lookup"><span data-stu-id="b8091-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="b8091-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="b8091-115">appProxy</span></span>|<span data-ttu-id="b8091-116">1</span><span class="sxs-lookup"><span data-stu-id="b8091-116">1</span></span>|<span data-ttu-id="b8091-117">Туннель трафика на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="b8091-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="b8091-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="b8091-118">packetTunnel</span></span>|<span data-ttu-id="b8091-119">2</span><span class="sxs-lookup"><span data-stu-id="b8091-119">2</span></span>|<span data-ttu-id="b8091-120">Туннель трафика на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="b8091-120">Tunnel traffic at the IP layer.</span></span>|




