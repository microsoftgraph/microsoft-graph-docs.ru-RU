---
title: Тип перечисления windowsPrivacyDataAccessLevel
description: Определите уровень доступа к определенной категории конфиденциальности данных Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64db5eb78708a0cfa835bd695ba01b2c267fc4fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959318"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="85f3c-103">Тип перечисления windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="85f3c-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="85f3c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85f3c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85f3c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85f3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85f3c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85f3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85f3c-107">Определите уровень доступа к определенной категории конфиденциальности данных Windows.</span><span class="sxs-lookup"><span data-stu-id="85f3c-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="85f3c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="85f3c-108">Members</span></span>
|<span data-ttu-id="85f3c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="85f3c-109">Member</span></span>|<span data-ttu-id="85f3c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="85f3c-110">Value</span></span>|<span data-ttu-id="85f3c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85f3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85f3c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="85f3c-112">notConfigured</span></span>|<span data-ttu-id="85f3c-113">0</span><span class="sxs-lookup"><span data-stu-id="85f3c-113">0</span></span>|<span data-ttu-id="85f3c-114">Уровень доступа не указан, не целей.</span><span class="sxs-lookup"><span data-stu-id="85f3c-114">No access level specified, no intents.</span></span> <span data-ttu-id="85f3c-115">Устройство может работать либо как и UserInControl или ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="85f3c-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="85f3c-116">Он может зависеть от конфиденциальности данных были обращении к ним версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="85f3c-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="85f3c-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="85f3c-117">forceAllow</span></span>|<span data-ttu-id="85f3c-118">1</span><span class="sxs-lookup"><span data-stu-id="85f3c-118">1</span></span>|<span data-ttu-id="85f3c-119">Приложения смогут получить доступ к данным указанного конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="85f3c-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="85f3c-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="85f3c-120">forceDeny</span></span>|<span data-ttu-id="85f3c-121">2</span><span class="sxs-lookup"><span data-stu-id="85f3c-121">2</span></span>|<span data-ttu-id="85f3c-122">Приложения будет запрещен доступ к данным указанного конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="85f3c-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="85f3c-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="85f3c-123">userInControl</span></span>|<span data-ttu-id="85f3c-124">3</span><span class="sxs-lookup"><span data-stu-id="85f3c-124">3</span></span>|<span data-ttu-id="85f3c-125">При попытке получить доступ к данным указанного конфиденциальности приложения будет предложено пользователей.</span><span class="sxs-lookup"><span data-stu-id="85f3c-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





