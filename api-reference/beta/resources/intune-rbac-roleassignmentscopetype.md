---
title: Тип перечисления roleAssignmentScopeType
description: Указывает тип области для назначения ролей.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b815cf7eb396aa82f49df792ceee0612678077c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419893"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="39d17-103">Тип перечисления roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="39d17-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="39d17-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39d17-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39d17-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39d17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39d17-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39d17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39d17-107">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="39d17-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="39d17-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="39d17-108">Members</span></span>
|<span data-ttu-id="39d17-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="39d17-109">Member</span></span>|<span data-ttu-id="39d17-110">Значение</span><span class="sxs-lookup"><span data-stu-id="39d17-110">Value</span></span>|<span data-ttu-id="39d17-111">Описание</span><span class="sxs-lookup"><span data-stu-id="39d17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39d17-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="39d17-112">resourceScope</span></span>|<span data-ttu-id="39d17-113">0</span><span class="sxs-lookup"><span data-stu-id="39d17-113">0</span></span>|<span data-ttu-id="39d17-114">Разрешить назначения для указанного ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="39d17-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="39d17-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="39d17-115">allDevices</span></span>|<span data-ttu-id="39d17-116">1</span><span class="sxs-lookup"><span data-stu-id="39d17-116">1</span></span>|<span data-ttu-id="39d17-117">Разрешить назначений на все устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="39d17-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="39d17-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="39d17-118">allLicensedUsers</span></span>|<span data-ttu-id="39d17-119">2</span><span class="sxs-lookup"><span data-stu-id="39d17-119">2</span></span>|<span data-ttu-id="39d17-120">Разрешить назначения для всех пользователей с корпоративным лицензированием Intune.</span><span class="sxs-lookup"><span data-stu-id="39d17-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="39d17-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="39d17-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="39d17-122">3</span><span class="sxs-lookup"><span data-stu-id="39d17-122">3</span></span>|<span data-ttu-id="39d17-123">Разрешить назначения для всех устройств Intune и лицензированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="39d17-123">Allow assignments to all Intune devices and licensed users.</span></span>|




