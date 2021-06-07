---
title: тип enum safeSearchFilterType
description: Указывает, какой уровень безопасного поиска (фильтрация контента для взрослых) требуется
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 60463edb06c961e7911b5391ea8b3e4e8f1150ec
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754701"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="2fe6a-103">тип enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="2fe6a-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="2fe6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fe6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fe6a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fe6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fe6a-106">Указывает, какой уровень безопасного поиска (фильтрация контента для взрослых) требуется</span><span class="sxs-lookup"><span data-stu-id="2fe6a-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="2fe6a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2fe6a-107">Members</span></span>
|<span data-ttu-id="2fe6a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2fe6a-108">Member</span></span>|<span data-ttu-id="2fe6a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2fe6a-109">Value</span></span>|<span data-ttu-id="2fe6a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2fe6a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fe6a-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="2fe6a-111">userDefined</span></span>|<span data-ttu-id="2fe6a-112">0</span><span class="sxs-lookup"><span data-stu-id="2fe6a-112">0</span></span>|<span data-ttu-id="2fe6a-113">Значение User Defined, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="2fe6a-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2fe6a-114">строгий</span><span class="sxs-lookup"><span data-stu-id="2fe6a-114">strict</span></span>|<span data-ttu-id="2fe6a-115">1</span><span class="sxs-lookup"><span data-stu-id="2fe6a-115">1</span></span>|<span data-ttu-id="2fe6a-116">Строгая, самая высокая фильтрация по отношению к контенту для взрослых.</span><span class="sxs-lookup"><span data-stu-id="2fe6a-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="2fe6a-117">умеренный</span><span class="sxs-lookup"><span data-stu-id="2fe6a-117">moderate</span></span>|<span data-ttu-id="2fe6a-118">2</span><span class="sxs-lookup"><span data-stu-id="2fe6a-118">2</span></span>|<span data-ttu-id="2fe6a-119">Умеренная фильтрация контента для взрослых (допустимые результаты поиска не будут фильтроваться).</span><span class="sxs-lookup"><span data-stu-id="2fe6a-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




