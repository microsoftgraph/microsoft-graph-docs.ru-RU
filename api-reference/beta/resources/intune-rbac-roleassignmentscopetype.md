---
title: тип перечисления Ролеассигнментскопетипе
description: Задает тип области для назначения роли.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efdbc48a1363ba9d958c8bfe0dd2889478975083
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773254"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="63b61-103">тип перечисления Ролеассигнментскопетипе</span><span class="sxs-lookup"><span data-stu-id="63b61-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="63b61-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63b61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63b61-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63b61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63b61-106">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="63b61-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="63b61-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="63b61-107">Members</span></span>
|<span data-ttu-id="63b61-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="63b61-108">Member</span></span>|<span data-ttu-id="63b61-109">Значение</span><span class="sxs-lookup"><span data-stu-id="63b61-109">Value</span></span>|<span data-ttu-id="63b61-110">Описание</span><span class="sxs-lookup"><span data-stu-id="63b61-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63b61-111">ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="63b61-111">resourceScope</span></span>|<span data-ttu-id="63b61-112">нуль</span><span class="sxs-lookup"><span data-stu-id="63b61-112">0</span></span>|<span data-ttu-id="63b61-113">Разрешить назначения для указанного Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="63b61-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="63b61-114">аллдевицес</span><span class="sxs-lookup"><span data-stu-id="63b61-114">allDevices</span></span>|<span data-ttu-id="63b61-115">1,1</span><span class="sxs-lookup"><span data-stu-id="63b61-115">1</span></span>|<span data-ttu-id="63b61-116">Разрешить назначения всем устройствам Intune.</span><span class="sxs-lookup"><span data-stu-id="63b61-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="63b61-117">алллиценседусерс</span><span class="sxs-lookup"><span data-stu-id="63b61-117">allLicensedUsers</span></span>|<span data-ttu-id="63b61-118">2</span><span class="sxs-lookup"><span data-stu-id="63b61-118">2</span></span>|<span data-ttu-id="63b61-119">Разрешить назначения всем пользователям, лицензированным в Intune.</span><span class="sxs-lookup"><span data-stu-id="63b61-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="63b61-120">аллдевицесандлиценседусерс</span><span class="sxs-lookup"><span data-stu-id="63b61-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="63b61-121">4</span><span class="sxs-lookup"><span data-stu-id="63b61-121">3</span></span>|<span data-ttu-id="63b61-122">Разрешает назначения всем устройствам Intune и лицензированным пользователям.</span><span class="sxs-lookup"><span data-stu-id="63b61-122">Allow assignments to all Intune devices and licensed users.</span></span>|



