---
title: тип перечисления Ролеассигнментскопетипе
description: Задает тип области для назначения роли.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9659c4eaa1f4080ef5dd07a5e69f76a7a14d50
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775690"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="9bcd8-103">тип перечисления Ролеассигнментскопетипе</span><span class="sxs-lookup"><span data-stu-id="9bcd8-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="9bcd8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bcd8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bcd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bcd8-106">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="9bcd8-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="9bcd8-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9bcd8-107">Members</span></span>
|<span data-ttu-id="9bcd8-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9bcd8-108">Member</span></span>|<span data-ttu-id="9bcd8-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9bcd8-109">Value</span></span>|<span data-ttu-id="9bcd8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9bcd8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bcd8-111">Ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="9bcd8-111">resourceScope</span></span>|<span data-ttu-id="9bcd8-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9bcd8-112">0</span></span>|<span data-ttu-id="9bcd8-113">Разрешить назначения для указанного Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="9bcd8-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="9bcd8-114">Аллдевицес</span><span class="sxs-lookup"><span data-stu-id="9bcd8-114">allDevices</span></span>|<span data-ttu-id="9bcd8-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9bcd8-115">1</span></span>|<span data-ttu-id="9bcd8-116">Разрешить назначения всем устройствам Intune.</span><span class="sxs-lookup"><span data-stu-id="9bcd8-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="9bcd8-117">Алллиценседусерс</span><span class="sxs-lookup"><span data-stu-id="9bcd8-117">allLicensedUsers</span></span>|<span data-ttu-id="9bcd8-118">2</span><span class="sxs-lookup"><span data-stu-id="9bcd8-118">2</span></span>|<span data-ttu-id="9bcd8-119">Разрешить назначения всем пользователям, лицензированным в Intune.</span><span class="sxs-lookup"><span data-stu-id="9bcd8-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="9bcd8-120">Аллдевицесандлиценседусерс</span><span class="sxs-lookup"><span data-stu-id="9bcd8-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="9bcd8-121">4</span><span class="sxs-lookup"><span data-stu-id="9bcd8-121">3</span></span>|<span data-ttu-id="9bcd8-122">Разрешает назначения всем устройствам Intune и лицензированным пользователям.</span><span class="sxs-lookup"><span data-stu-id="9bcd8-122">Allow assignments to all Intune devices and licensed users.</span></span>|





