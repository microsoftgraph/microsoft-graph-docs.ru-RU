---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 98508a288ef46f8112ac5d796b8ddef64c5940e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058202"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="eee97-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="eee97-103">edgeKioskModeRestrictionType enum type</span></span>

<span data-ttu-id="eee97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eee97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eee97-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eee97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eee97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eee97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eee97-107">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="eee97-107">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="eee97-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="eee97-108">Members</span></span>
|<span data-ttu-id="eee97-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="eee97-109">Member</span></span>|<span data-ttu-id="eee97-110">Значение</span><span class="sxs-lookup"><span data-stu-id="eee97-110">Value</span></span>|<span data-ttu-id="eee97-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eee97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eee97-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="eee97-112">notConfigured</span></span>|<span data-ttu-id="eee97-113">нуль</span><span class="sxs-lookup"><span data-stu-id="eee97-113">0</span></span>|<span data-ttu-id="eee97-114">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="eee97-114">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="eee97-115">дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="eee97-115">digitalSignage</span></span>|<span data-ttu-id="eee97-116">1 </span><span class="sxs-lookup"><span data-stu-id="eee97-116">1</span></span>|<span data-ttu-id="eee97-117">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="eee97-117">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="eee97-118">нормалмоде</span><span class="sxs-lookup"><span data-stu-id="eee97-118">normalMode</span></span>|<span data-ttu-id="eee97-119">2 </span><span class="sxs-lookup"><span data-stu-id="eee97-119">2</span></span>|<span data-ttu-id="eee97-120">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="eee97-120">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="eee97-121">публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="eee97-121">publicBrowsingSingleApp</span></span>|<span data-ttu-id="eee97-122">4</span><span class="sxs-lookup"><span data-stu-id="eee97-122">3</span></span>|<span data-ttu-id="eee97-123">Общедоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="eee97-123">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="eee97-124">публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="eee97-124">publicBrowsingMultiApp</span></span>|<span data-ttu-id="eee97-125">4 </span><span class="sxs-lookup"><span data-stu-id="eee97-125">4</span></span>|<span data-ttu-id="eee97-126">Общедоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="eee97-126">Public browsing (inPrivate) in multi-app mode.</span></span>|






