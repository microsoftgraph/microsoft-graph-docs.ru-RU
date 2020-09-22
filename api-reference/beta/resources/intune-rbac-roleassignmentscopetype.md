---
title: тип перечисления Ролеассигнментскопетипе
description: Задает тип области для назначения роли.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 16781d47a9db63bd346c4c33efe3cbcdd278a5e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039519"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="74ee6-103">тип перечисления Ролеассигнментскопетипе</span><span class="sxs-lookup"><span data-stu-id="74ee6-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="74ee6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74ee6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74ee6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ee6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74ee6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74ee6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74ee6-107">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="74ee6-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="74ee6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="74ee6-108">Members</span></span>
|<span data-ttu-id="74ee6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="74ee6-109">Member</span></span>|<span data-ttu-id="74ee6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="74ee6-110">Value</span></span>|<span data-ttu-id="74ee6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74ee6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74ee6-112">ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="74ee6-112">resourceScope</span></span>|<span data-ttu-id="74ee6-113">нуль</span><span class="sxs-lookup"><span data-stu-id="74ee6-113">0</span></span>|<span data-ttu-id="74ee6-114">Разрешить назначения для указанного Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="74ee6-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="74ee6-115">аллдевицес</span><span class="sxs-lookup"><span data-stu-id="74ee6-115">allDevices</span></span>|<span data-ttu-id="74ee6-116">1 </span><span class="sxs-lookup"><span data-stu-id="74ee6-116">1</span></span>|<span data-ttu-id="74ee6-117">Разрешить назначения всем устройствам Intune.</span><span class="sxs-lookup"><span data-stu-id="74ee6-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="74ee6-118">алллиценседусерс</span><span class="sxs-lookup"><span data-stu-id="74ee6-118">allLicensedUsers</span></span>|<span data-ttu-id="74ee6-119">2 </span><span class="sxs-lookup"><span data-stu-id="74ee6-119">2</span></span>|<span data-ttu-id="74ee6-120">Разрешить назначения всем пользователям, лицензированным в Intune.</span><span class="sxs-lookup"><span data-stu-id="74ee6-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="74ee6-121">аллдевицесандлиценседусерс</span><span class="sxs-lookup"><span data-stu-id="74ee6-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="74ee6-122">4</span><span class="sxs-lookup"><span data-stu-id="74ee6-122">3</span></span>|<span data-ttu-id="74ee6-123">Разрешает назначения всем устройствам Intune и лицензированным пользователям.</span><span class="sxs-lookup"><span data-stu-id="74ee6-123">Allow assignments to all Intune devices and licensed users.</span></span>|






