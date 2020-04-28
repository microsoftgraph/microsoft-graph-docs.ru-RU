---
title: тип перечисления Впнтраффикрулеапптипе
description: Указывает тип приложения, с которым связано правило трафика VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cad0ab3a49c6139707fb30c703cc670be6bc5f7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43359003"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="245d8-103">тип перечисления Впнтраффикрулеапптипе</span><span class="sxs-lookup"><span data-stu-id="245d8-103">vpnTrafficRuleAppType enum type</span></span>

<span data-ttu-id="245d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="245d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="245d8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="245d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="245d8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="245d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="245d8-107">Указывает тип приложения, с которым связано правило трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="245d8-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="245d8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="245d8-108">Members</span></span>
|<span data-ttu-id="245d8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="245d8-109">Member</span></span>|<span data-ttu-id="245d8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="245d8-110">Value</span></span>|<span data-ttu-id="245d8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="245d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="245d8-112">Нет</span><span class="sxs-lookup"><span data-stu-id="245d8-112">none</span></span>|<span data-ttu-id="245d8-113">нуль</span><span class="sxs-lookup"><span data-stu-id="245d8-113">0</span></span>|<span data-ttu-id="245d8-114">Правило трафика не связано с приложением.</span><span class="sxs-lookup"><span data-stu-id="245d8-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="245d8-115">системной</span><span class="sxs-lookup"><span data-stu-id="245d8-115">desktop</span></span>|<span data-ttu-id="245d8-116">1,1</span><span class="sxs-lookup"><span data-stu-id="245d8-116">1</span></span>|<span data-ttu-id="245d8-117">Правило трафика связано с классическим приложением.</span><span class="sxs-lookup"><span data-stu-id="245d8-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="245d8-118">Гринвич</span><span class="sxs-lookup"><span data-stu-id="245d8-118">universal</span></span>|<span data-ttu-id="245d8-119">2</span><span class="sxs-lookup"><span data-stu-id="245d8-119">2</span></span>|<span data-ttu-id="245d8-120">Правило трафика связано с универсальным приложением.</span><span class="sxs-lookup"><span data-stu-id="245d8-120">The traffic rule is associated with a Universal app.</span></span>|



