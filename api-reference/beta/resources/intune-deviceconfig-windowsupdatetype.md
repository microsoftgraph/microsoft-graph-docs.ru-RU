---
title: тип перечисления Виндовсупдатетипе
description: Какие устройства филиала будут получать обновления от
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 41a6d23e42d263dd8241e960af693450ac0a7c3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369509"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="ec6da-103">тип перечисления Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="ec6da-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="ec6da-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec6da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec6da-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec6da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec6da-106">Какие устройства филиала будут получать обновления от</span><span class="sxs-lookup"><span data-stu-id="ec6da-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="ec6da-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ec6da-107">Members</span></span>
|<span data-ttu-id="ec6da-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ec6da-108">Member</span></span>|<span data-ttu-id="ec6da-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ec6da-109">Value</span></span>|<span data-ttu-id="ec6da-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ec6da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec6da-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="ec6da-111">userDefined</span></span>|<span data-ttu-id="ec6da-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ec6da-112">0</span></span>|<span data-ttu-id="ec6da-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="ec6da-113">Allow the user to set.</span></span>|
|<span data-ttu-id="ec6da-114">ко</span><span class="sxs-lookup"><span data-stu-id="ec6da-114">all</span></span>|<span data-ttu-id="ec6da-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ec6da-115">1</span></span>|<span data-ttu-id="ec6da-116">Половина ежегодного канала (нацеленная).</span><span class="sxs-lookup"><span data-stu-id="ec6da-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="ec6da-117">Device получает все подходящее обновление компонентов из Полугодого канала (нацелено).</span><span class="sxs-lookup"><span data-stu-id="ec6da-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="ec6da-118">бусинессреадйонли</span><span class="sxs-lookup"><span data-stu-id="ec6da-118">businessReadyOnly</span></span>|<span data-ttu-id="ec6da-119">2</span><span class="sxs-lookup"><span data-stu-id="ec6da-119">2</span></span>|<span data-ttu-id="ec6da-120">Половина ежегодного канала.</span><span class="sxs-lookup"><span data-stu-id="ec6da-120">Semi-annual Channel.</span></span> <span data-ttu-id="ec6da-121">Устройство получает обновления компонентов из Полугодого канала.</span><span class="sxs-lookup"><span data-stu-id="ec6da-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="ec6da-122">виндовсинсидербуилдфаст</span><span class="sxs-lookup"><span data-stu-id="ec6da-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="ec6da-123">4</span><span class="sxs-lookup"><span data-stu-id="ec6da-123">3</span></span>|<span data-ttu-id="ec6da-124">Предварительная сборка Windows для предварительной сборки — Быстрая</span><span class="sxs-lookup"><span data-stu-id="ec6da-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="ec6da-125">виндовсинсидербуилдслов</span><span class="sxs-lookup"><span data-stu-id="ec6da-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="ec6da-126">SP4</span><span class="sxs-lookup"><span data-stu-id="ec6da-126">4</span></span>|<span data-ttu-id="ec6da-127">Сборка для предварительной оценки Windows — низкая</span><span class="sxs-lookup"><span data-stu-id="ec6da-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="ec6da-128">виндовсинсидербуилдрелеасе</span><span class="sxs-lookup"><span data-stu-id="ec6da-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="ec6da-129">17:00</span><span class="sxs-lookup"><span data-stu-id="ec6da-129">5</span></span>|<span data-ttu-id="ec6da-130">Выпуск сборки предварительной оценки Windows</span><span class="sxs-lookup"><span data-stu-id="ec6da-130">Release Windows Insider build</span></span>|



