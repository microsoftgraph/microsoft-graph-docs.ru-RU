---
title: тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе
description: Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 55092376dcf0d5e4ae72b5cb6f607cf984959c4d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797180"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="23907-103">тип перечисления Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="23907-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="23907-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23907-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23907-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23907-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23907-106">Возможные значения для состояний политики автоматического обновления приложений на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="23907-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="23907-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="23907-107">Members</span></span>
|<span data-ttu-id="23907-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="23907-108">Member</span></span>|<span data-ttu-id="23907-109">Значение</span><span class="sxs-lookup"><span data-stu-id="23907-109">Value</span></span>|<span data-ttu-id="23907-110">Описание</span><span class="sxs-lookup"><span data-stu-id="23907-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23907-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="23907-111">notConfigured</span></span>|<span data-ttu-id="23907-112">нуль</span><span class="sxs-lookup"><span data-stu-id="23907-112">0</span></span>|<span data-ttu-id="23907-113">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="23907-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="23907-114">усерчоице</span><span class="sxs-lookup"><span data-stu-id="23907-114">userChoice</span></span>|<span data-ttu-id="23907-115">1,1</span><span class="sxs-lookup"><span data-stu-id="23907-115">1</span></span>|<span data-ttu-id="23907-116">Пользователь может управлять автоматическим обновлением.</span><span class="sxs-lookup"><span data-stu-id="23907-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="23907-117">ключа</span><span class="sxs-lookup"><span data-stu-id="23907-117">never</span></span>|<span data-ttu-id="23907-118">2</span><span class="sxs-lookup"><span data-stu-id="23907-118">2</span></span>|<span data-ttu-id="23907-119">Приложения никогда не обновляются автоматически.</span><span class="sxs-lookup"><span data-stu-id="23907-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="23907-120">вифионли</span><span class="sxs-lookup"><span data-stu-id="23907-120">wiFiOnly</span></span>|<span data-ttu-id="23907-121">4</span><span class="sxs-lookup"><span data-stu-id="23907-121">3</span></span>|<span data-ttu-id="23907-122">Приложения автоматически обновляются только с помощью Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="23907-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="23907-123">Постоянное</span><span class="sxs-lookup"><span data-stu-id="23907-123">always</span></span>|<span data-ttu-id="23907-124">4 </span><span class="sxs-lookup"><span data-stu-id="23907-124">4</span></span>|<span data-ttu-id="23907-125">Приложения автоматически обновляются в любое время.</span><span class="sxs-lookup"><span data-stu-id="23907-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="23907-126">Может взиматься плата за передачу данных.</span><span class="sxs-lookup"><span data-stu-id="23907-126">Data charges may apply.</span></span>|



