---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 402feb76fbb95664f5b4fe8190dfb71504db0abf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791879"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="1cd0c-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="1cd0c-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="1cd0c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cd0c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cd0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cd0c-106">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="1cd0c-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="1cd0c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1cd0c-107">Members</span></span>
|<span data-ttu-id="1cd0c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1cd0c-108">Member</span></span>|<span data-ttu-id="1cd0c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1cd0c-109">Value</span></span>|<span data-ttu-id="1cd0c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1cd0c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd0c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1cd0c-111">notConfigured</span></span>|<span data-ttu-id="1cd0c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1cd0c-112">0</span></span>|<span data-ttu-id="1cd0c-113">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="1cd0c-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="1cd0c-114">дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="1cd0c-114">digitalSignage</span></span>|<span data-ttu-id="1cd0c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="1cd0c-115">1</span></span>|<span data-ttu-id="1cd0c-116">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd0c-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="1cd0c-117">нормалмоде</span><span class="sxs-lookup"><span data-stu-id="1cd0c-117">normalMode</span></span>|<span data-ttu-id="1cd0c-118">2</span><span class="sxs-lookup"><span data-stu-id="1cd0c-118">2</span></span>|<span data-ttu-id="1cd0c-119">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="1cd0c-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="1cd0c-120">публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="1cd0c-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="1cd0c-121">4</span><span class="sxs-lookup"><span data-stu-id="1cd0c-121">3</span></span>|<span data-ttu-id="1cd0c-122">Общедоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd0c-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="1cd0c-123">публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="1cd0c-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="1cd0c-124">4 </span><span class="sxs-lookup"><span data-stu-id="1cd0c-124">4</span></span>|<span data-ttu-id="1cd0c-125">Общедоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="1cd0c-125">Public browsing (inPrivate) in multi-app mode.</span></span>|



