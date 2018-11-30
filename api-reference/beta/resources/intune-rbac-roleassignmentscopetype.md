---
title: Тип перечисления roleAssignmentScopeType
description: Указывает тип области для назначения ролей.
ms.openlocfilehash: dcfac7b345dde2d8f107b8ec756d017966a6a94a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080032"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="d2de6-103">Тип перечисления roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="d2de6-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="d2de6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2de6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2de6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2de6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2de6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2de6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2de6-107">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="d2de6-107">Specifies the type of scope for a Role Assignment.</span></span>
## <a name="members"></a><span data-ttu-id="d2de6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d2de6-108">Members</span></span>
|<span data-ttu-id="d2de6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d2de6-109">Member</span></span>|<span data-ttu-id="d2de6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d2de6-110">Value</span></span>|<span data-ttu-id="d2de6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d2de6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2de6-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="d2de6-112">resourceScope</span></span>|<span data-ttu-id="d2de6-113">0</span><span class="sxs-lookup"><span data-stu-id="d2de6-113">0</span></span>|<span data-ttu-id="d2de6-114">Разрешить назначения для указанного ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="d2de6-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="d2de6-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="d2de6-115">allDevices</span></span>|<span data-ttu-id="d2de6-116">1</span><span class="sxs-lookup"><span data-stu-id="d2de6-116">1</span></span>|<span data-ttu-id="d2de6-117">Разрешить назначений на все устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="d2de6-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="d2de6-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="d2de6-118">allLicensedUsers</span></span>|<span data-ttu-id="d2de6-119">2</span><span class="sxs-lookup"><span data-stu-id="d2de6-119">2</span></span>|<span data-ttu-id="d2de6-120">Разрешить назначения для всех пользователей с корпоративным лицензированием Intune.</span><span class="sxs-lookup"><span data-stu-id="d2de6-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="d2de6-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="d2de6-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="d2de6-122">3</span><span class="sxs-lookup"><span data-stu-id="d2de6-122">3</span></span>|<span data-ttu-id="d2de6-123">Разрешить назначения для всех устройств Intune и лицензированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="d2de6-123">Allow assignments to all Intune devices and licensed users.</span></span>|





