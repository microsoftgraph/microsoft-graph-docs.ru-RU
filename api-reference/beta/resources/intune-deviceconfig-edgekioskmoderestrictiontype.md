---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74b03555456c058411c9a50c7392f29fe60d3aed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524514"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="7ba42-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="7ba42-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="7ba42-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ba42-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ba42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ba42-106">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="7ba42-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="7ba42-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7ba42-107">Members</span></span>
|<span data-ttu-id="7ba42-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7ba42-108">Member</span></span>|<span data-ttu-id="7ba42-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7ba42-109">Value</span></span>|<span data-ttu-id="7ba42-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ba42-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba42-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7ba42-111">notConfigured</span></span>|<span data-ttu-id="7ba42-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7ba42-112">0</span></span>|<span data-ttu-id="7ba42-113">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="7ba42-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="7ba42-114">Дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="7ba42-114">digitalSignage</span></span>|<span data-ttu-id="7ba42-115">1 </span><span class="sxs-lookup"><span data-stu-id="7ba42-115">1</span></span>|<span data-ttu-id="7ba42-116">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="7ba42-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="7ba42-117">Нормалмоде</span><span class="sxs-lookup"><span data-stu-id="7ba42-117">normalMode</span></span>|<span data-ttu-id="7ba42-118">2 </span><span class="sxs-lookup"><span data-stu-id="7ba42-118">2</span></span>|<span data-ttu-id="7ba42-119">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="7ba42-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="7ba42-120">Публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="7ba42-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="7ba42-121">3 </span><span class="sxs-lookup"><span data-stu-id="7ba42-121">3</span></span>|<span data-ttu-id="7ba42-122">ОбщеДоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="7ba42-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="7ba42-123">Публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="7ba42-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="7ba42-124">4 </span><span class="sxs-lookup"><span data-stu-id="7ba42-124">4</span></span>|<span data-ttu-id="7ba42-125">ОбщеДоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="7ba42-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





