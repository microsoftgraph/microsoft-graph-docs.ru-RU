---
title: тип перечисления Ролеассигнментскопетипе
description: Задает тип области для назначения роли.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3205b3ffb451f6ab62e7573e94a4347491a0c7cb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259139"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="59824-103">тип перечисления Ролеассигнментскопетипе</span><span class="sxs-lookup"><span data-stu-id="59824-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="59824-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59824-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59824-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59824-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59824-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59824-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59824-107">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="59824-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="59824-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="59824-108">Members</span></span>
|<span data-ttu-id="59824-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="59824-109">Member</span></span>|<span data-ttu-id="59824-110">Значение</span><span class="sxs-lookup"><span data-stu-id="59824-110">Value</span></span>|<span data-ttu-id="59824-111">Описание</span><span class="sxs-lookup"><span data-stu-id="59824-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59824-112">ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="59824-112">resourceScope</span></span>|<span data-ttu-id="59824-113">нуль</span><span class="sxs-lookup"><span data-stu-id="59824-113">0</span></span>|<span data-ttu-id="59824-114">Разрешить назначения для указанного Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="59824-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="59824-115">аллдевицес</span><span class="sxs-lookup"><span data-stu-id="59824-115">allDevices</span></span>|<span data-ttu-id="59824-116">1,1</span><span class="sxs-lookup"><span data-stu-id="59824-116">1</span></span>|<span data-ttu-id="59824-117">Разрешить назначения всем устройствам Intune.</span><span class="sxs-lookup"><span data-stu-id="59824-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="59824-118">алллиценседусерс</span><span class="sxs-lookup"><span data-stu-id="59824-118">allLicensedUsers</span></span>|<span data-ttu-id="59824-119">2</span><span class="sxs-lookup"><span data-stu-id="59824-119">2</span></span>|<span data-ttu-id="59824-120">Разрешить назначения всем пользователям, лицензированным в Intune.</span><span class="sxs-lookup"><span data-stu-id="59824-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="59824-121">аллдевицесандлиценседусерс</span><span class="sxs-lookup"><span data-stu-id="59824-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="59824-122">4</span><span class="sxs-lookup"><span data-stu-id="59824-122">3</span></span>|<span data-ttu-id="59824-123">Разрешает назначения всем устройствам Intune и лицензированным пользователям.</span><span class="sxs-lookup"><span data-stu-id="59824-123">Allow assignments to all Intune devices and licensed users.</span></span>|




