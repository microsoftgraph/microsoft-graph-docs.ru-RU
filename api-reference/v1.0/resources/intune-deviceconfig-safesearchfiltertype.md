---
title: Тип перечисления safeSearchFilterType
description: Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 788a266cdd0161ce1cfef426a7fcf4d9726e3324
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964615"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="c427b-103">Тип перечисления safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="c427b-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="c427b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c427b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c427b-105">Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="c427b-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="c427b-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c427b-106">Members</span></span>
|<span data-ttu-id="c427b-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c427b-107">Member</span></span>|<span data-ttu-id="c427b-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c427b-108">Value</span></span>|<span data-ttu-id="c427b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c427b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c427b-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="c427b-110">userDefined</span></span>|<span data-ttu-id="c427b-111">0</span><span class="sxs-lookup"><span data-stu-id="c427b-111">0</span></span>|<span data-ttu-id="c427b-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="c427b-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c427b-113">строгое</span><span class="sxs-lookup"><span data-stu-id="c427b-113">strict</span></span>|<span data-ttu-id="c427b-114">1</span><span class="sxs-lookup"><span data-stu-id="c427b-114">1</span></span>|<span data-ttu-id="c427b-115">Строгий, наибольший фильтрации содержимое для взрослых.</span><span class="sxs-lookup"><span data-stu-id="c427b-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="c427b-116">от среднего</span><span class="sxs-lookup"><span data-stu-id="c427b-116">moderate</span></span>|<span data-ttu-id="c427b-117">2</span><span class="sxs-lookup"><span data-stu-id="c427b-117">2</span></span>|<span data-ttu-id="c427b-118">От среднего фильтрации содержимое для взрослых (результаты поиска допустимый не фильтруются).</span><span class="sxs-lookup"><span data-stu-id="c427b-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



