---
title: Тип перечисления windowsPrivacyDataAccessLevel
description: Определите уровень доступа к определенной категории конфиденциальности данных Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d6fed0897b22a6a6b478dc5d2b7954faca42b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410625"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="3d2db-103">Тип перечисления windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="3d2db-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="3d2db-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3d2db-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d2db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d2db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d2db-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d2db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d2db-107">Определите уровень доступа к определенной категории конфиденциальности данных Windows.</span><span class="sxs-lookup"><span data-stu-id="3d2db-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="3d2db-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3d2db-108">Members</span></span>
|<span data-ttu-id="3d2db-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3d2db-109">Member</span></span>|<span data-ttu-id="3d2db-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3d2db-110">Value</span></span>|<span data-ttu-id="3d2db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3d2db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d2db-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3d2db-112">notConfigured</span></span>|<span data-ttu-id="3d2db-113">0</span><span class="sxs-lookup"><span data-stu-id="3d2db-113">0</span></span>|<span data-ttu-id="3d2db-114">Уровень доступа не указан, не целей.</span><span class="sxs-lookup"><span data-stu-id="3d2db-114">No access level specified, no intents.</span></span> <span data-ttu-id="3d2db-115">Устройство может работать либо как и UserInControl или ForceAllow.</span><span class="sxs-lookup"><span data-stu-id="3d2db-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="3d2db-116">Он может зависеть от конфиденциальности данных были обращении к ним версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="3d2db-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="3d2db-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="3d2db-117">forceAllow</span></span>|<span data-ttu-id="3d2db-118">1</span><span class="sxs-lookup"><span data-stu-id="3d2db-118">1</span></span>|<span data-ttu-id="3d2db-119">Приложения смогут получить доступ к данным указанного конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3d2db-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="3d2db-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="3d2db-120">forceDeny</span></span>|<span data-ttu-id="3d2db-121">2</span><span class="sxs-lookup"><span data-stu-id="3d2db-121">2</span></span>|<span data-ttu-id="3d2db-122">Приложения будет запрещен доступ к данным указанного конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3d2db-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="3d2db-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="3d2db-123">userInControl</span></span>|<span data-ttu-id="3d2db-124">3</span><span class="sxs-lookup"><span data-stu-id="3d2db-124">3</span></span>|<span data-ttu-id="3d2db-125">При попытке получить доступ к данным указанного конфиденциальности приложения будет предложено пользователей.</span><span class="sxs-lookup"><span data-stu-id="3d2db-125">Users will be prompted when apps try to access specified privacy data.</span></span>|




