---
title: тип перечисления Ролеассигнментскопетипе
description: Задает тип области для назначения роли.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f30ad6480d2791c0c8469f6886e9b7002b6c1c6e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709861"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="45555-103">тип перечисления Ролеассигнментскопетипе</span><span class="sxs-lookup"><span data-stu-id="45555-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="45555-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45555-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45555-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45555-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45555-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45555-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45555-107">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="45555-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="45555-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="45555-108">Members</span></span>
|<span data-ttu-id="45555-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="45555-109">Member</span></span>|<span data-ttu-id="45555-110">Значение</span><span class="sxs-lookup"><span data-stu-id="45555-110">Value</span></span>|<span data-ttu-id="45555-111">Описание</span><span class="sxs-lookup"><span data-stu-id="45555-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45555-112">ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="45555-112">resourceScope</span></span>|<span data-ttu-id="45555-113">нуль</span><span class="sxs-lookup"><span data-stu-id="45555-113">0</span></span>|<span data-ttu-id="45555-114">Разрешить назначения для указанного Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="45555-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="45555-115">аллдевицес</span><span class="sxs-lookup"><span data-stu-id="45555-115">allDevices</span></span>|<span data-ttu-id="45555-116">1,1</span><span class="sxs-lookup"><span data-stu-id="45555-116">1</span></span>|<span data-ttu-id="45555-117">Разрешить назначения всем устройствам Intune.</span><span class="sxs-lookup"><span data-stu-id="45555-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="45555-118">алллиценседусерс</span><span class="sxs-lookup"><span data-stu-id="45555-118">allLicensedUsers</span></span>|<span data-ttu-id="45555-119">2</span><span class="sxs-lookup"><span data-stu-id="45555-119">2</span></span>|<span data-ttu-id="45555-120">Разрешить назначения всем пользователям, лицензированным в Intune.</span><span class="sxs-lookup"><span data-stu-id="45555-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="45555-121">аллдевицесандлиценседусерс</span><span class="sxs-lookup"><span data-stu-id="45555-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="45555-122">4</span><span class="sxs-lookup"><span data-stu-id="45555-122">3</span></span>|<span data-ttu-id="45555-123">Разрешает назначения всем устройствам Intune и лицензированным пользователям.</span><span class="sxs-lookup"><span data-stu-id="45555-123">Allow assignments to all Intune devices and licensed users.</span></span>|





