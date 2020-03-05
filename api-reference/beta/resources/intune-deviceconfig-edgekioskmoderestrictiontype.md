---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 929e74097d329f2d6932ae3aadaa001258dbd2fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530056"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="45966-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="45966-103">edgeKioskModeRestrictionType enum type</span></span>

<span data-ttu-id="45966-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="45966-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45966-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45966-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45966-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45966-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45966-107">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="45966-107">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="45966-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="45966-108">Members</span></span>
|<span data-ttu-id="45966-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="45966-109">Member</span></span>|<span data-ttu-id="45966-110">Значение</span><span class="sxs-lookup"><span data-stu-id="45966-110">Value</span></span>|<span data-ttu-id="45966-111">Описание</span><span class="sxs-lookup"><span data-stu-id="45966-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45966-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="45966-112">notConfigured</span></span>|<span data-ttu-id="45966-113">нуль</span><span class="sxs-lookup"><span data-stu-id="45966-113">0</span></span>|<span data-ttu-id="45966-114">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="45966-114">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="45966-115">дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="45966-115">digitalSignage</span></span>|<span data-ttu-id="45966-116">1 </span><span class="sxs-lookup"><span data-stu-id="45966-116">1</span></span>|<span data-ttu-id="45966-117">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="45966-117">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="45966-118">нормалмоде</span><span class="sxs-lookup"><span data-stu-id="45966-118">normalMode</span></span>|<span data-ttu-id="45966-119">2 </span><span class="sxs-lookup"><span data-stu-id="45966-119">2</span></span>|<span data-ttu-id="45966-120">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="45966-120">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="45966-121">публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="45966-121">publicBrowsingSingleApp</span></span>|<span data-ttu-id="45966-122">3 </span><span class="sxs-lookup"><span data-stu-id="45966-122">3</span></span>|<span data-ttu-id="45966-123">Общедоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="45966-123">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="45966-124">публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="45966-124">publicBrowsingMultiApp</span></span>|<span data-ttu-id="45966-125">4 </span><span class="sxs-lookup"><span data-stu-id="45966-125">4</span></span>|<span data-ttu-id="45966-126">Общедоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="45966-126">Public browsing (inPrivate) in multi-app mode.</span></span>|



