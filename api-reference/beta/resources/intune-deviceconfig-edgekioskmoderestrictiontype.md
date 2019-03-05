---
title: тип перечисления Еджекиоскмодерестриктионтипе
description: Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0dcd1d30895acbdecf9d9cc706ee14b7907f14f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177961"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="17f7a-103">тип перечисления Еджекиоскмодерестриктионтипе</span><span class="sxs-lookup"><span data-stu-id="17f7a-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="17f7a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17f7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17f7a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17f7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17f7a-106">Укажите, как параметры Microsoft Edge будут ограничены в зависимости от режима киоска.</span><span class="sxs-lookup"><span data-stu-id="17f7a-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="17f7a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="17f7a-107">Members</span></span>
|<span data-ttu-id="17f7a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="17f7a-108">Member</span></span>|<span data-ttu-id="17f7a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="17f7a-109">Value</span></span>|<span data-ttu-id="17f7a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="17f7a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17f7a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="17f7a-111">notConfigured</span></span>|<span data-ttu-id="17f7a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="17f7a-112">0</span></span>|<span data-ttu-id="17f7a-113">Не настроено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="17f7a-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="17f7a-114">Дигиталсигнаже</span><span class="sxs-lookup"><span data-stu-id="17f7a-114">digitalSignage</span></span>|<span data-ttu-id="17f7a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="17f7a-115">1</span></span>|<span data-ttu-id="17f7a-116">Интерактивная и цифровая подпись в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="17f7a-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="17f7a-117">Нормалмоде</span><span class="sxs-lookup"><span data-stu-id="17f7a-117">normalMode</span></span>|<span data-ttu-id="17f7a-118">2</span><span class="sxs-lookup"><span data-stu-id="17f7a-118">2</span></span>|<span data-ttu-id="17f7a-119">В обычном режиме (полная версия Microsoft EDGE).</span><span class="sxs-lookup"><span data-stu-id="17f7a-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="17f7a-120">Публикбровсингсинглеапп</span><span class="sxs-lookup"><span data-stu-id="17f7a-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="17f7a-121">4</span><span class="sxs-lookup"><span data-stu-id="17f7a-121">3</span></span>|<span data-ttu-id="17f7a-122">ОбщеДоступный обзор в режиме одного приложения.</span><span class="sxs-lookup"><span data-stu-id="17f7a-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="17f7a-123">Публикбровсингмултиапп</span><span class="sxs-lookup"><span data-stu-id="17f7a-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="17f7a-124">4</span><span class="sxs-lookup"><span data-stu-id="17f7a-124">4</span></span>|<span data-ttu-id="17f7a-125">ОбщеДоступный обзор (InPrivate) в режиме нескольких приложений.</span><span class="sxs-lookup"><span data-stu-id="17f7a-125">Public browsing (inPrivate) in multi-app mode.</span></span>|




