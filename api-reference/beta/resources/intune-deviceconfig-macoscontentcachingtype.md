---
title: тип перечисления Макосконтенткачингтипе
description: Указывает тип контента, который может кэшироваться службой кэширования контента Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9022b320507cc10455e2eeb3ebd3a3ca58d52f71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993842"
---
# <a name="macoscontentcachingtype-enum-type"></a><span data-ttu-id="79ba0-103">тип перечисления Макосконтенткачингтипе</span><span class="sxs-lookup"><span data-stu-id="79ba0-103">macOSContentCachingType enum type</span></span>

<span data-ttu-id="79ba0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79ba0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79ba0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ba0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79ba0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79ba0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79ba0-107">Указывает тип контента, который может кэшироваться службой кэширования контента Apple.</span><span class="sxs-lookup"><span data-stu-id="79ba0-107">Indicates the type of content allowed to be cached by Apple's content caching service.</span></span>

## <a name="members"></a><span data-ttu-id="79ba0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="79ba0-108">Members</span></span>
|<span data-ttu-id="79ba0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="79ba0-109">Member</span></span>|<span data-ttu-id="79ba0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="79ba0-110">Value</span></span>|<span data-ttu-id="79ba0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="79ba0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ba0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="79ba0-112">notConfigured</span></span>|<span data-ttu-id="79ba0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="79ba0-113">0</span></span>|<span data-ttu-id="79ba0-114">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="79ba0-114">Default.</span></span> <span data-ttu-id="79ba0-115">Будут кэшироваться данные пользователя в iCloud и данных, не являющихся iCloud.</span><span class="sxs-lookup"><span data-stu-id="79ba0-115">Both user iCloud data and non-iCloud data will be cached.</span></span>|
|<span data-ttu-id="79ba0-116">усерконтентонли</span><span class="sxs-lookup"><span data-stu-id="79ba0-116">userContentOnly</span></span>|<span data-ttu-id="79ba0-117">1 </span><span class="sxs-lookup"><span data-stu-id="79ba0-117">1</span></span>|<span data-ttu-id="79ba0-118">Разрешить службе кэширования контента Apple кэшировать данные пользователя в iCloud.</span><span class="sxs-lookup"><span data-stu-id="79ba0-118">Allow Apple's content caching service to cache user iCloud data.</span></span>|
|<span data-ttu-id="79ba0-119">шаредконтентонли</span><span class="sxs-lookup"><span data-stu-id="79ba0-119">sharedContentOnly</span></span>|<span data-ttu-id="79ba0-120">2 </span><span class="sxs-lookup"><span data-stu-id="79ba0-120">2</span></span>|<span data-ttu-id="79ba0-121">Разрешить службе кэширования контента Apple кэшировать данные, не относящиеся к iCloud (например, приложения и обновления программного обеспечения).</span><span class="sxs-lookup"><span data-stu-id="79ba0-121">Allow Apple's content caching service to cache non-iCloud data (e.g. app and software updates).</span></span>|






