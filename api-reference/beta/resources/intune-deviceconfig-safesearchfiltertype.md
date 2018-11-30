---
title: Тип перечисления safeSearchFilterType
description: Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным
ms.openlocfilehash: 71a59574fd98e2571a33e58415acb612f32326a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076064"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="c52df-103">Тип перечисления safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="c52df-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="c52df-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c52df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c52df-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c52df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c52df-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c52df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c52df-107">Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="c52df-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="c52df-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c52df-108">Members</span></span>
|<span data-ttu-id="c52df-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c52df-109">Member</span></span>|<span data-ttu-id="c52df-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c52df-110">Value</span></span>|<span data-ttu-id="c52df-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c52df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c52df-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="c52df-112">userDefined</span></span>|<span data-ttu-id="c52df-113">0</span><span class="sxs-lookup"><span data-stu-id="c52df-113">0</span></span>|<span data-ttu-id="c52df-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="c52df-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c52df-115">строгое</span><span class="sxs-lookup"><span data-stu-id="c52df-115">strict</span></span>|<span data-ttu-id="c52df-116">1</span><span class="sxs-lookup"><span data-stu-id="c52df-116">1</span></span>|<span data-ttu-id="c52df-117">Строгий, наибольший фильтрации содержимое для взрослых.</span><span class="sxs-lookup"><span data-stu-id="c52df-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="c52df-118">от среднего</span><span class="sxs-lookup"><span data-stu-id="c52df-118">moderate</span></span>|<span data-ttu-id="c52df-119">2</span><span class="sxs-lookup"><span data-stu-id="c52df-119">2</span></span>|<span data-ttu-id="c52df-120">От среднего фильтрации содержимое для взрослых (результаты поиска допустимый не фильтруются).</span><span class="sxs-lookup"><span data-stu-id="c52df-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





