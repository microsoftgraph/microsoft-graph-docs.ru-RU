---
title: тип перечисления Ролеассигнментскопетипе
description: Задает тип области для назначения роли.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f922cf51729f178ab9ca94db127efb5b70bb94fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523895"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="a6733-103">тип перечисления Ролеассигнментскопетипе</span><span class="sxs-lookup"><span data-stu-id="a6733-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="a6733-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a6733-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6733-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6733-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6733-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6733-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6733-107">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a6733-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="a6733-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a6733-108">Members</span></span>
|<span data-ttu-id="a6733-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a6733-109">Member</span></span>|<span data-ttu-id="a6733-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a6733-110">Value</span></span>|<span data-ttu-id="a6733-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a6733-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6733-112">ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="a6733-112">resourceScope</span></span>|<span data-ttu-id="a6733-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a6733-113">0</span></span>|<span data-ttu-id="a6733-114">Разрешить назначения для указанного Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="a6733-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="a6733-115">аллдевицес</span><span class="sxs-lookup"><span data-stu-id="a6733-115">allDevices</span></span>|<span data-ttu-id="a6733-116">1 </span><span class="sxs-lookup"><span data-stu-id="a6733-116">1</span></span>|<span data-ttu-id="a6733-117">Разрешить назначения всем устройствам Intune.</span><span class="sxs-lookup"><span data-stu-id="a6733-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="a6733-118">алллиценседусерс</span><span class="sxs-lookup"><span data-stu-id="a6733-118">allLicensedUsers</span></span>|<span data-ttu-id="a6733-119">2 </span><span class="sxs-lookup"><span data-stu-id="a6733-119">2</span></span>|<span data-ttu-id="a6733-120">Разрешить назначения всем пользователям, лицензированным в Intune.</span><span class="sxs-lookup"><span data-stu-id="a6733-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="a6733-121">аллдевицесандлиценседусерс</span><span class="sxs-lookup"><span data-stu-id="a6733-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="a6733-122">3 </span><span class="sxs-lookup"><span data-stu-id="a6733-122">3</span></span>|<span data-ttu-id="a6733-123">Разрешает назначения всем устройствам Intune и лицензированным пользователям.</span><span class="sxs-lookup"><span data-stu-id="a6733-123">Allow assignments to all Intune devices and licensed users.</span></span>|



