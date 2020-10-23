---
title: тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе
description: Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 41ff774e30342b12e7ba8de8d1583039565c2540
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691458"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="7e0b0-103">тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="7e0b0-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="7e0b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e0b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e0b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e0b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e0b0-107">Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="7e0b0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7e0b0-108">Members</span></span>
|<span data-ttu-id="7e0b0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7e0b0-109">Member</span></span>|<span data-ttu-id="7e0b0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7e0b0-110">Value</span></span>|<span data-ttu-id="7e0b0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7e0b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e0b0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7e0b0-112">notConfigured</span></span>|<span data-ttu-id="7e0b0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="7e0b0-113">0</span></span>|<span data-ttu-id="7e0b0-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="7e0b0-115">усерчоице</span><span class="sxs-lookup"><span data-stu-id="7e0b0-115">userChoice</span></span>|<span data-ttu-id="7e0b0-116">1,1</span><span class="sxs-lookup"><span data-stu-id="7e0b0-116">1</span></span>|<span data-ttu-id="7e0b0-117">Пользователь может управлять автоматическим обновлением.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="7e0b0-118">ключа</span><span class="sxs-lookup"><span data-stu-id="7e0b0-118">never</span></span>|<span data-ttu-id="7e0b0-119">2</span><span class="sxs-lookup"><span data-stu-id="7e0b0-119">2</span></span>|<span data-ttu-id="7e0b0-120">Приложения никогда не обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="7e0b0-121">вифионли</span><span class="sxs-lookup"><span data-stu-id="7e0b0-121">wiFiOnly</span></span>|<span data-ttu-id="7e0b0-122">4</span><span class="sxs-lookup"><span data-stu-id="7e0b0-122">3</span></span>|<span data-ttu-id="7e0b0-123">Приложения автоматически обновляются только на Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="7e0b0-124">Постоянное</span><span class="sxs-lookup"><span data-stu-id="7e0b0-124">always</span></span>|<span data-ttu-id="7e0b0-125">4 </span><span class="sxs-lookup"><span data-stu-id="7e0b0-125">4</span></span>|<span data-ttu-id="7e0b0-126">Приложения автоматически обновляются в любое время.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="7e0b0-127">Может взиматься плата за передачу данных.</span><span class="sxs-lookup"><span data-stu-id="7e0b0-127">Data charges may apply.</span></span>|





