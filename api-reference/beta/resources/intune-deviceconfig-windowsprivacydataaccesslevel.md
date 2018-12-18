---
title: Тип перечисления windowsPrivacyDataAccessLevel
description: Определите уровень доступа к определенной категории конфиденциальности данных Windows.
author: tfitzmac
ms.openlocfilehash: 6eb1c1ea6eff28d90979da3ff998fd8442df353a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332412"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="6bc61-103">Тип перечисления windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="6bc61-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="6bc61-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6bc61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bc61-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bc61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bc61-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6bc61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bc61-107">Определите уровень доступа к определенной категории конфиденциальности данных Windows.</span><span class="sxs-lookup"><span data-stu-id="6bc61-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="6bc61-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6bc61-108">Members</span></span>
|<span data-ttu-id="6bc61-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6bc61-109">Member</span></span>|<span data-ttu-id="6bc61-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6bc61-110">Value</span></span>|<span data-ttu-id="6bc61-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6bc61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc61-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6bc61-112">notConfigured</span></span>|<span data-ttu-id="6bc61-113">0</span><span class="sxs-lookup"><span data-stu-id="6bc61-113">0</span></span>|<span data-ttu-id="6bc61-114">Уровень доступа не указан, не целей.</span><span class="sxs-lookup"><span data-stu-id="6bc61-114">No access level specified, no intents.</span></span> <span data-ttu-id="6bc61-115">Устройство может работать либо как и UserInControl или ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="6bc61-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="6bc61-116">Он может зависеть от конфиденциальности данных были обращении к ним версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="6bc61-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="6bc61-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="6bc61-117">forceAllow</span></span>|<span data-ttu-id="6bc61-118">1</span><span class="sxs-lookup"><span data-stu-id="6bc61-118">1</span></span>|<span data-ttu-id="6bc61-119">Приложения смогут получить доступ к данным указанного конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6bc61-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="6bc61-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="6bc61-120">forceDeny</span></span>|<span data-ttu-id="6bc61-121">2</span><span class="sxs-lookup"><span data-stu-id="6bc61-121">2</span></span>|<span data-ttu-id="6bc61-122">Приложения будет запрещен доступ к данным указанного конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6bc61-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="6bc61-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="6bc61-123">userInControl</span></span>|<span data-ttu-id="6bc61-124">3</span><span class="sxs-lookup"><span data-stu-id="6bc61-124">3</span></span>|<span data-ttu-id="6bc61-125">При попытке получить доступ к данным указанного конфиденциальности приложения будет предложено пользователей.</span><span class="sxs-lookup"><span data-stu-id="6bc61-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





