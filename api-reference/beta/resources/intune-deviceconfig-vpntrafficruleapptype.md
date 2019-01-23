---
title: Тип перечисления vpnTrafficRuleAppType
description: Указывает тип приложения, с которым связана правило трафика через VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 061cb5701830939576f5b9a649c73b4d44eada18
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396023"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="ec63c-103">Тип перечисления vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="ec63c-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="ec63c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ec63c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ec63c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec63c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec63c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec63c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec63c-107">Указывает тип приложения, с которым связана правило трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="ec63c-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="ec63c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ec63c-108">Members</span></span>
|<span data-ttu-id="ec63c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ec63c-109">Member</span></span>|<span data-ttu-id="ec63c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ec63c-110">Value</span></span>|<span data-ttu-id="ec63c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ec63c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec63c-112">none</span><span class="sxs-lookup"><span data-stu-id="ec63c-112">none</span></span>|<span data-ttu-id="ec63c-113">0</span><span class="sxs-lookup"><span data-stu-id="ec63c-113">0</span></span>|<span data-ttu-id="ec63c-114">Правила трафика не связан с приложения.</span><span class="sxs-lookup"><span data-stu-id="ec63c-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="ec63c-115">рабочий стол</span><span class="sxs-lookup"><span data-stu-id="ec63c-115">desktop</span></span>|<span data-ttu-id="ec63c-116">1</span><span class="sxs-lookup"><span data-stu-id="ec63c-116">1</span></span>|<span data-ttu-id="ec63c-117">Трафик правило связано с помощью классического приложения.</span><span class="sxs-lookup"><span data-stu-id="ec63c-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="ec63c-118">Универсальные</span><span class="sxs-lookup"><span data-stu-id="ec63c-118">universal</span></span>|<span data-ttu-id="ec63c-119">2</span><span class="sxs-lookup"><span data-stu-id="ec63c-119">2</span></span>|<span data-ttu-id="ec63c-120">Трафик правило связано с помощью универсального приложения.</span><span class="sxs-lookup"><span data-stu-id="ec63c-120">The traffic rule is associated with a Universal app.</span></span>|




