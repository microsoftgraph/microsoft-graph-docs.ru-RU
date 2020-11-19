---
title: тип перечисления Дефендераттакксурфацетипе
description: Возможные значения правил уменьшения зоны атак защитника
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 435ce477f60f14437a05e22fd5c670cbe1b25796
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256654"
---
# <a name="defenderattacksurfacetype-enum-type"></a><span data-ttu-id="a7b53-103">тип перечисления Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="a7b53-103">defenderAttackSurfaceType enum type</span></span>

<span data-ttu-id="a7b53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7b53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7b53-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7b53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7b53-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7b53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7b53-107">Возможные значения правил уменьшения зоны атак защитника</span><span class="sxs-lookup"><span data-stu-id="a7b53-107">Possible values of Defender Attack Surface Reduction Rules</span></span>

## <a name="members"></a><span data-ttu-id="a7b53-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a7b53-108">Members</span></span>
|<span data-ttu-id="a7b53-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a7b53-109">Member</span></span>|<span data-ttu-id="a7b53-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a7b53-110">Value</span></span>|<span data-ttu-id="a7b53-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a7b53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7b53-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="a7b53-112">userDefined</span></span>|<span data-ttu-id="a7b53-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a7b53-113">0</span></span>|<span data-ttu-id="a7b53-114">Значение по умолчанию, которое отключает правило сокращения для уязвимой зоны.</span><span class="sxs-lookup"><span data-stu-id="a7b53-114">Default, which disables attack surface reduction rule.</span></span>|
|<span data-ttu-id="a7b53-115">блок</span><span class="sxs-lookup"><span data-stu-id="a7b53-115">block</span></span>|<span data-ttu-id="a7b53-116">1,1</span><span class="sxs-lookup"><span data-stu-id="a7b53-116">1</span></span>|<span data-ttu-id="a7b53-117">Включите правило сокращения для уязвимой зоны.</span><span class="sxs-lookup"><span data-stu-id="a7b53-117">Enable the attack surface reduction rule.</span></span>|
|<span data-ttu-id="a7b53-118">аудитмоде</span><span class="sxs-lookup"><span data-stu-id="a7b53-118">auditMode</span></span>|<span data-ttu-id="a7b53-119">2</span><span class="sxs-lookup"><span data-stu-id="a7b53-119">2</span></span>|<span data-ttu-id="a7b53-120">Оцените, как правило ASR будет влиять на вашу организацию, если она включена.</span><span class="sxs-lookup"><span data-stu-id="a7b53-120">Evaluate how the ASR rule would impact your organization if enabled.</span></span> <span data-ttu-id="a7b53-121">Не изменяет функциональность, но создает журналы.</span><span class="sxs-lookup"><span data-stu-id="a7b53-121">Does not change functionality but generate logs.</span></span>|
|<span data-ttu-id="a7b53-122">пользователя</span><span class="sxs-lookup"><span data-stu-id="a7b53-122">warn</span></span>|<span data-ttu-id="a7b53-123">6 </span><span class="sxs-lookup"><span data-stu-id="a7b53-123">6</span></span>|<span data-ttu-id="a7b53-124">Предупреждающее сообщение о том, что пользователь может обходить блок из правила уменьшения уязвимой зоны.</span><span class="sxs-lookup"><span data-stu-id="a7b53-124">Warning message to end user with ability to bypass block from attack surface reduction rule.</span></span>|
|<span data-ttu-id="a7b53-125">отключение</span><span class="sxs-lookup"><span data-stu-id="a7b53-125">disable</span></span>|<span data-ttu-id="a7b53-126">99</span><span class="sxs-lookup"><span data-stu-id="a7b53-126">99</span></span>|<span data-ttu-id="a7b53-127">Отключение правила уменьшения уязвимой зоны</span><span class="sxs-lookup"><span data-stu-id="a7b53-127">Disable the attack surface reduction rule</span></span>|




