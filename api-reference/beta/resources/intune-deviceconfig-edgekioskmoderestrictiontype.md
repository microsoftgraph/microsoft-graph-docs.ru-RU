---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ff024dd8cd27872d0895068fba42e0018fdce011
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332514"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="920ca-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="920ca-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="920ca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="920ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="920ca-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="920ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="920ca-106">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="920ca-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="920ca-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="920ca-107">Members</span></span>
|<span data-ttu-id="920ca-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="920ca-108">Member</span></span>|<span data-ttu-id="920ca-109">Значение</span><span class="sxs-lookup"><span data-stu-id="920ca-109">Value</span></span>|<span data-ttu-id="920ca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="920ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="920ca-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="920ca-111">notConfigured</span></span>|<span data-ttu-id="920ca-112">нуль</span><span class="sxs-lookup"><span data-stu-id="920ca-112">0</span></span>|<span data-ttu-id="920ca-113">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="920ca-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="920ca-114">дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="920ca-114">digitalSignage</span></span>|<span data-ttu-id="920ca-115">1,1</span><span class="sxs-lookup"><span data-stu-id="920ca-115">1</span></span>|<span data-ttu-id="920ca-116">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="920ca-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="920ca-117">нормалмоде</span><span class="sxs-lookup"><span data-stu-id="920ca-117">normalMode</span></span>|<span data-ttu-id="920ca-118">2</span><span class="sxs-lookup"><span data-stu-id="920ca-118">2</span></span>|<span data-ttu-id="920ca-119">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="920ca-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="920ca-120">публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="920ca-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="920ca-121">4</span><span class="sxs-lookup"><span data-stu-id="920ca-121">3</span></span>|<span data-ttu-id="920ca-122">Общедоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="920ca-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="920ca-123">публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="920ca-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="920ca-124">SP4</span><span class="sxs-lookup"><span data-stu-id="920ca-124">4</span></span>|<span data-ttu-id="920ca-125">Общедоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="920ca-125">Public browsing (inPrivate) in multi-app mode.</span></span>|



