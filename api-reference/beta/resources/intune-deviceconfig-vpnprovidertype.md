---
title: тип перечисления Впнпровидертипе
description: Тип поставщика для VPN каждого приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ea4dee71a18a6ddca4519d8b421d2097fc7907b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367647"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="ab476-103">тип перечисления Впнпровидертипе</span><span class="sxs-lookup"><span data-stu-id="ab476-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="ab476-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab476-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab476-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab476-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab476-106">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="ab476-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="ab476-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ab476-107">Members</span></span>
|<span data-ttu-id="ab476-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ab476-108">Member</span></span>|<span data-ttu-id="ab476-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ab476-109">Value</span></span>|<span data-ttu-id="ab476-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ab476-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab476-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ab476-111">notConfigured</span></span>|<span data-ttu-id="ab476-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ab476-112">0</span></span>|<span data-ttu-id="ab476-113">Туннельный трафик не настраивается явным образом.</span><span class="sxs-lookup"><span data-stu-id="ab476-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="ab476-114">апппрокси</span><span class="sxs-lookup"><span data-stu-id="ab476-114">appProxy</span></span>|<span data-ttu-id="ab476-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ab476-115">1</span></span>|<span data-ttu-id="ab476-116">Трафик туннеля на уровне приложения.</span><span class="sxs-lookup"><span data-stu-id="ab476-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="ab476-117">паккеттуннел</span><span class="sxs-lookup"><span data-stu-id="ab476-117">packetTunnel</span></span>|<span data-ttu-id="ab476-118">2</span><span class="sxs-lookup"><span data-stu-id="ab476-118">2</span></span>|<span data-ttu-id="ab476-119">Трафик туннеля на уровне IP.</span><span class="sxs-lookup"><span data-stu-id="ab476-119">Tunnel traffic at the IP layer.</span></span>|



