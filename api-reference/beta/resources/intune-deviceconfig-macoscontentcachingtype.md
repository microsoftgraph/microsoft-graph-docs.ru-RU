---
title: тип перечисления Макосконтенткачингтипе
description: Указывает тип контента, который может кэшироваться службой кэширования контента Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a79cd14a6bd765f260439a259c63106e6211cacc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268736"
---
# <a name="macoscontentcachingtype-enum-type"></a><span data-ttu-id="907c7-103">тип перечисления Макосконтенткачингтипе</span><span class="sxs-lookup"><span data-stu-id="907c7-103">macOSContentCachingType enum type</span></span>

<span data-ttu-id="907c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="907c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="907c7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="907c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="907c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="907c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="907c7-107">Указывает тип контента, который может кэшироваться службой кэширования контента Apple.</span><span class="sxs-lookup"><span data-stu-id="907c7-107">Indicates the type of content allowed to be cached by Apple's content caching service.</span></span>

## <a name="members"></a><span data-ttu-id="907c7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="907c7-108">Members</span></span>
|<span data-ttu-id="907c7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="907c7-109">Member</span></span>|<span data-ttu-id="907c7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="907c7-110">Value</span></span>|<span data-ttu-id="907c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="907c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="907c7-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="907c7-112">notConfigured</span></span>|<span data-ttu-id="907c7-113">нуль</span><span class="sxs-lookup"><span data-stu-id="907c7-113">0</span></span>|<span data-ttu-id="907c7-114">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="907c7-114">Default.</span></span> <span data-ttu-id="907c7-115">Будут кэшироваться данные пользователя в iCloud и данных, не являющихся iCloud.</span><span class="sxs-lookup"><span data-stu-id="907c7-115">Both user iCloud data and non-iCloud data will be cached.</span></span>|
|<span data-ttu-id="907c7-116">усерконтентонли</span><span class="sxs-lookup"><span data-stu-id="907c7-116">userContentOnly</span></span>|<span data-ttu-id="907c7-117">1,1</span><span class="sxs-lookup"><span data-stu-id="907c7-117">1</span></span>|<span data-ttu-id="907c7-118">Разрешить службе кэширования контента Apple кэшировать данные пользователя в iCloud.</span><span class="sxs-lookup"><span data-stu-id="907c7-118">Allow Apple's content caching service to cache user iCloud data.</span></span>|
|<span data-ttu-id="907c7-119">шаредконтентонли</span><span class="sxs-lookup"><span data-stu-id="907c7-119">sharedContentOnly</span></span>|<span data-ttu-id="907c7-120">2</span><span class="sxs-lookup"><span data-stu-id="907c7-120">2</span></span>|<span data-ttu-id="907c7-121">Разрешить службе кэширования контента Apple кэшировать данные, не относящиеся к iCloud (например, приложения и обновления программного обеспечения).</span><span class="sxs-lookup"><span data-stu-id="907c7-121">Allow Apple's content caching service to cache non-iCloud data (e.g. app and software updates).</span></span>|




