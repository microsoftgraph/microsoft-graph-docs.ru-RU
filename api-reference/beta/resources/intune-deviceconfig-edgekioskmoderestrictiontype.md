---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014025b04974df90dc6e22e55f3597fc265b207d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946744"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="116a7-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="116a7-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="116a7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="116a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="116a7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="116a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="116a7-106">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="116a7-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="116a7-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="116a7-107">Members</span></span>
|<span data-ttu-id="116a7-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="116a7-108">Member</span></span>|<span data-ttu-id="116a7-109">Значение</span><span class="sxs-lookup"><span data-stu-id="116a7-109">Value</span></span>|<span data-ttu-id="116a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="116a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="116a7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="116a7-111">notConfigured</span></span>|<span data-ttu-id="116a7-112">нуль</span><span class="sxs-lookup"><span data-stu-id="116a7-112">0</span></span>|<span data-ttu-id="116a7-113">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="116a7-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="116a7-114">Дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="116a7-114">digitalSignage</span></span>|<span data-ttu-id="116a7-115">1,1</span><span class="sxs-lookup"><span data-stu-id="116a7-115">1</span></span>|<span data-ttu-id="116a7-116">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="116a7-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="116a7-117">Нормалмоде</span><span class="sxs-lookup"><span data-stu-id="116a7-117">normalMode</span></span>|<span data-ttu-id="116a7-118">2</span><span class="sxs-lookup"><span data-stu-id="116a7-118">2</span></span>|<span data-ttu-id="116a7-119">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="116a7-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="116a7-120">Публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="116a7-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="116a7-121">4</span><span class="sxs-lookup"><span data-stu-id="116a7-121">3</span></span>|<span data-ttu-id="116a7-122">Общедоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="116a7-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="116a7-123">Публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="116a7-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="116a7-124">SP4</span><span class="sxs-lookup"><span data-stu-id="116a7-124">4</span></span>|<span data-ttu-id="116a7-125">Общедоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="116a7-125">Public browsing (inPrivate) in multi-app mode.</span></span>|




