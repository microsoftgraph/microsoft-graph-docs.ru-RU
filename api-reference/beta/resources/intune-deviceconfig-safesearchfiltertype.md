---
title: тип перечисления Сафесеарчфилтертипе
description: Указывает, какой уровень безопасного поиска (фильтрация содержимого для взрослых) является обязательным
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 22b87cdb9cf4b5ea96caab7efa764de0f27fa452
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787595"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="709d5-103">тип перечисления Сафесеарчфилтертипе</span><span class="sxs-lookup"><span data-stu-id="709d5-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="709d5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="709d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="709d5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="709d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="709d5-106">Указывает, какой уровень безопасного поиска (фильтрация содержимого для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="709d5-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="709d5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="709d5-107">Members</span></span>
|<span data-ttu-id="709d5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="709d5-108">Member</span></span>|<span data-ttu-id="709d5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="709d5-109">Value</span></span>|<span data-ttu-id="709d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="709d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="709d5-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="709d5-111">userDefined</span></span>|<span data-ttu-id="709d5-112">нуль</span><span class="sxs-lookup"><span data-stu-id="709d5-112">0</span></span>|<span data-ttu-id="709d5-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="709d5-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="709d5-114">жестк</span><span class="sxs-lookup"><span data-stu-id="709d5-114">strict</span></span>|<span data-ttu-id="709d5-115">1,1</span><span class="sxs-lookup"><span data-stu-id="709d5-115">1</span></span>|<span data-ttu-id="709d5-116">Максимальная фильтрация с использованием содержимого для взрослых.</span><span class="sxs-lookup"><span data-stu-id="709d5-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="709d5-117">средние</span><span class="sxs-lookup"><span data-stu-id="709d5-117">moderate</span></span>|<span data-ttu-id="709d5-118">2</span><span class="sxs-lookup"><span data-stu-id="709d5-118">2</span></span>|<span data-ttu-id="709d5-119">Умеренная фильтрация содержимого для взрослых (допустимые результаты поиска не будут фильтроваться).</span><span class="sxs-lookup"><span data-stu-id="709d5-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



