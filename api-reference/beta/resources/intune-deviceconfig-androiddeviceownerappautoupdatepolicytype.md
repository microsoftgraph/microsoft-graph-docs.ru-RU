---
title: тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе
description: Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cd003c8213faf45453f1b6165931181250c861ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487202"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="5c480-103">тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="5c480-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="5c480-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5c480-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c480-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c480-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c480-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c480-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c480-107">Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="5c480-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="5c480-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5c480-108">Members</span></span>
|<span data-ttu-id="5c480-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5c480-109">Member</span></span>|<span data-ttu-id="5c480-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5c480-110">Value</span></span>|<span data-ttu-id="5c480-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5c480-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c480-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5c480-112">notConfigured</span></span>|<span data-ttu-id="5c480-113">нуль</span><span class="sxs-lookup"><span data-stu-id="5c480-113">0</span></span>|<span data-ttu-id="5c480-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="5c480-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="5c480-115">усерчоице</span><span class="sxs-lookup"><span data-stu-id="5c480-115">userChoice</span></span>|<span data-ttu-id="5c480-116">1 </span><span class="sxs-lookup"><span data-stu-id="5c480-116">1</span></span>|<span data-ttu-id="5c480-117">Пользователь может управлять автоматическим обновлением.</span><span class="sxs-lookup"><span data-stu-id="5c480-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="5c480-118">ключа</span><span class="sxs-lookup"><span data-stu-id="5c480-118">never</span></span>|<span data-ttu-id="5c480-119">2 </span><span class="sxs-lookup"><span data-stu-id="5c480-119">2</span></span>|<span data-ttu-id="5c480-120">Приложения никогда не обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="5c480-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="5c480-121">вифионли</span><span class="sxs-lookup"><span data-stu-id="5c480-121">wiFiOnly</span></span>|<span data-ttu-id="5c480-122">3 </span><span class="sxs-lookup"><span data-stu-id="5c480-122">3</span></span>|<span data-ttu-id="5c480-123">Приложения автоматически обновляются только с помощью Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="5c480-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="5c480-124">Постоянное</span><span class="sxs-lookup"><span data-stu-id="5c480-124">always</span></span>|<span data-ttu-id="5c480-125">4 </span><span class="sxs-lookup"><span data-stu-id="5c480-125">4</span></span>|<span data-ttu-id="5c480-126">Приложения автоматически обновляются в любое время.</span><span class="sxs-lookup"><span data-stu-id="5c480-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="5c480-127">Может взиматься плата за передачу данных.</span><span class="sxs-lookup"><span data-stu-id="5c480-127">Data charges may apply.</span></span>|



