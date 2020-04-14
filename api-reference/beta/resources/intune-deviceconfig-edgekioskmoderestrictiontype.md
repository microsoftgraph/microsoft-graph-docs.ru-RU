---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1dfd86f9bd3a35e82f5210294c9b0648a4bab228
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386270"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="97ec6-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="97ec6-103">edgeKioskModeRestrictionType enum type</span></span>

<span data-ttu-id="97ec6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97ec6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97ec6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97ec6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97ec6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97ec6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97ec6-107">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="97ec6-107">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="97ec6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="97ec6-108">Members</span></span>
|<span data-ttu-id="97ec6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="97ec6-109">Member</span></span>|<span data-ttu-id="97ec6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="97ec6-110">Value</span></span>|<span data-ttu-id="97ec6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="97ec6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97ec6-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="97ec6-112">notConfigured</span></span>|<span data-ttu-id="97ec6-113">нуль</span><span class="sxs-lookup"><span data-stu-id="97ec6-113">0</span></span>|<span data-ttu-id="97ec6-114">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="97ec6-114">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="97ec6-115">дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="97ec6-115">digitalSignage</span></span>|<span data-ttu-id="97ec6-116">1,1</span><span class="sxs-lookup"><span data-stu-id="97ec6-116">1</span></span>|<span data-ttu-id="97ec6-117">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="97ec6-117">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="97ec6-118">нормалмоде</span><span class="sxs-lookup"><span data-stu-id="97ec6-118">normalMode</span></span>|<span data-ttu-id="97ec6-119">2</span><span class="sxs-lookup"><span data-stu-id="97ec6-119">2</span></span>|<span data-ttu-id="97ec6-120">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="97ec6-120">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="97ec6-121">публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="97ec6-121">publicBrowsingSingleApp</span></span>|<span data-ttu-id="97ec6-122">4</span><span class="sxs-lookup"><span data-stu-id="97ec6-122">3</span></span>|<span data-ttu-id="97ec6-123">Общедоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="97ec6-123">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="97ec6-124">публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="97ec6-124">publicBrowsingMultiApp</span></span>|<span data-ttu-id="97ec6-125">4 </span><span class="sxs-lookup"><span data-stu-id="97ec6-125">4</span></span>|<span data-ttu-id="97ec6-126">Общедоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="97ec6-126">Public browsing (inPrivate) in multi-app mode.</span></span>|



