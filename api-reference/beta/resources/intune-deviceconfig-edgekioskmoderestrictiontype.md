---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbd3d13ad39b6acda5fd67d69c8cb2de2f2e7c55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001469"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="c0bdb-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="c0bdb-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="c0bdb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0bdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0bdb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0bdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0bdb-106">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="c0bdb-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="c0bdb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c0bdb-107">Members</span></span>
|<span data-ttu-id="c0bdb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c0bdb-108">Member</span></span>|<span data-ttu-id="c0bdb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c0bdb-109">Value</span></span>|<span data-ttu-id="c0bdb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c0bdb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0bdb-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c0bdb-111">notConfigured</span></span>|<span data-ttu-id="c0bdb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c0bdb-112">0</span></span>|<span data-ttu-id="c0bdb-113">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="c0bdb-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="c0bdb-114">Дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="c0bdb-114">digitalSignage</span></span>|<span data-ttu-id="c0bdb-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c0bdb-115">1</span></span>|<span data-ttu-id="c0bdb-116">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="c0bdb-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="c0bdb-117">Нормалмоде</span><span class="sxs-lookup"><span data-stu-id="c0bdb-117">normalMode</span></span>|<span data-ttu-id="c0bdb-118">2</span><span class="sxs-lookup"><span data-stu-id="c0bdb-118">2</span></span>|<span data-ttu-id="c0bdb-119">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="c0bdb-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="c0bdb-120">Публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="c0bdb-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="c0bdb-121">4</span><span class="sxs-lookup"><span data-stu-id="c0bdb-121">3</span></span>|<span data-ttu-id="c0bdb-122">Общедоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="c0bdb-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="c0bdb-123">Публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="c0bdb-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="c0bdb-124">SP4</span><span class="sxs-lookup"><span data-stu-id="c0bdb-124">4</span></span>|<span data-ttu-id="c0bdb-125">Общедоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="c0bdb-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





