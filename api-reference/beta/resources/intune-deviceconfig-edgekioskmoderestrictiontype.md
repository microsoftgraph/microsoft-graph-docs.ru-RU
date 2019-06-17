---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dc2aa6dbea5e5fc068691c7de878321047c967d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989828"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="2464d-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="2464d-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="2464d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2464d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2464d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2464d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2464d-106">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="2464d-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="2464d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2464d-107">Members</span></span>
|<span data-ttu-id="2464d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2464d-108">Member</span></span>|<span data-ttu-id="2464d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2464d-109">Value</span></span>|<span data-ttu-id="2464d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2464d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2464d-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2464d-111">notConfigured</span></span>|<span data-ttu-id="2464d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2464d-112">0</span></span>|<span data-ttu-id="2464d-113">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="2464d-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="2464d-114">Дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="2464d-114">digitalSignage</span></span>|<span data-ttu-id="2464d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="2464d-115">1</span></span>|<span data-ttu-id="2464d-116">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="2464d-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="2464d-117">Нормалмоде</span><span class="sxs-lookup"><span data-stu-id="2464d-117">normalMode</span></span>|<span data-ttu-id="2464d-118">2</span><span class="sxs-lookup"><span data-stu-id="2464d-118">2</span></span>|<span data-ttu-id="2464d-119">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="2464d-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="2464d-120">Публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="2464d-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="2464d-121">4</span><span class="sxs-lookup"><span data-stu-id="2464d-121">3</span></span>|<span data-ttu-id="2464d-122">Общедоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="2464d-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="2464d-123">Публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="2464d-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="2464d-124">SP4</span><span class="sxs-lookup"><span data-stu-id="2464d-124">4</span></span>|<span data-ttu-id="2464d-125">Общедоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="2464d-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





