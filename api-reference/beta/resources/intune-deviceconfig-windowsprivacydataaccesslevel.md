---
title: Тип перечисления windowsPrivacyDataAccessLevel
description: Определите уровень доступа к определенной категории конфиденциальности данных Windows.
ms.openlocfilehash: 09db03706795cc2aba4cc0c93dce87dc7069cd3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082575"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="59711-103">Тип перечисления windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="59711-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="59711-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="59711-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59711-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59711-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59711-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59711-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59711-107">Определите уровень доступа к определенной категории конфиденциальности данных Windows.</span><span class="sxs-lookup"><span data-stu-id="59711-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="59711-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="59711-108">Members</span></span>
|<span data-ttu-id="59711-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="59711-109">Member</span></span>|<span data-ttu-id="59711-110">Значение</span><span class="sxs-lookup"><span data-stu-id="59711-110">Value</span></span>|<span data-ttu-id="59711-111">Description</span><span class="sxs-lookup"><span data-stu-id="59711-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59711-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="59711-112">notConfigured</span></span>|<span data-ttu-id="59711-113">0</span><span class="sxs-lookup"><span data-stu-id="59711-113">0</span></span>|<span data-ttu-id="59711-114">Уровень доступа не указан, не целей.</span><span class="sxs-lookup"><span data-stu-id="59711-114">No access level specified, no intents.</span></span> <span data-ttu-id="59711-115">Устройство может работать либо как и UserInControl или ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="59711-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="59711-116">Он может зависеть от конфиденциальности данных были обращении к ним версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="59711-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="59711-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="59711-117">forceAllow</span></span>|<span data-ttu-id="59711-118">1</span><span class="sxs-lookup"><span data-stu-id="59711-118">1</span></span>|<span data-ttu-id="59711-119">Приложения смогут получить доступ к данным указанного конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="59711-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="59711-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="59711-120">forceDeny</span></span>|<span data-ttu-id="59711-121">2</span><span class="sxs-lookup"><span data-stu-id="59711-121">2</span></span>|<span data-ttu-id="59711-122">Приложения будет запрещен доступ к данным указанного конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="59711-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="59711-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="59711-123">userInControl</span></span>|<span data-ttu-id="59711-124">3</span><span class="sxs-lookup"><span data-stu-id="59711-124">3</span></span>|<span data-ttu-id="59711-125">При попытке получить доступ к данным указанного конфиденциальности приложения будет предложено пользователей.</span><span class="sxs-lookup"><span data-stu-id="59711-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





