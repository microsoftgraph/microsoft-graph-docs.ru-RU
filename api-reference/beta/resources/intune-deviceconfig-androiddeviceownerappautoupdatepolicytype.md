---
title: тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе
description: Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8fd84350d9685a65dc53e803fc55b7238bfa9908
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470913"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="bf474-103">тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="bf474-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="bf474-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf474-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf474-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf474-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf474-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf474-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf474-107">Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="bf474-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="bf474-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bf474-108">Members</span></span>
|<span data-ttu-id="bf474-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bf474-109">Member</span></span>|<span data-ttu-id="bf474-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bf474-110">Value</span></span>|<span data-ttu-id="bf474-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf474-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf474-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bf474-112">notConfigured</span></span>|<span data-ttu-id="bf474-113">нуль</span><span class="sxs-lookup"><span data-stu-id="bf474-113">0</span></span>|<span data-ttu-id="bf474-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="bf474-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="bf474-115">усерчоице</span><span class="sxs-lookup"><span data-stu-id="bf474-115">userChoice</span></span>|<span data-ttu-id="bf474-116">1,1</span><span class="sxs-lookup"><span data-stu-id="bf474-116">1</span></span>|<span data-ttu-id="bf474-117">Пользователь может управлять автоматическим обновлением.</span><span class="sxs-lookup"><span data-stu-id="bf474-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="bf474-118">ключа</span><span class="sxs-lookup"><span data-stu-id="bf474-118">never</span></span>|<span data-ttu-id="bf474-119">2</span><span class="sxs-lookup"><span data-stu-id="bf474-119">2</span></span>|<span data-ttu-id="bf474-120">Приложения никогда не обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="bf474-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="bf474-121">вифионли</span><span class="sxs-lookup"><span data-stu-id="bf474-121">wiFiOnly</span></span>|<span data-ttu-id="bf474-122">4</span><span class="sxs-lookup"><span data-stu-id="bf474-122">3</span></span>|<span data-ttu-id="bf474-123">Приложения автоматически обновляются только с помощью Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="bf474-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="bf474-124">Постоянное</span><span class="sxs-lookup"><span data-stu-id="bf474-124">always</span></span>|<span data-ttu-id="bf474-125">4 </span><span class="sxs-lookup"><span data-stu-id="bf474-125">4</span></span>|<span data-ttu-id="bf474-126">Приложения автоматически обновляются в любое время.</span><span class="sxs-lookup"><span data-stu-id="bf474-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="bf474-127">Может взиматься плата за передачу данных.</span><span class="sxs-lookup"><span data-stu-id="bf474-127">Data charges may apply.</span></span>|



