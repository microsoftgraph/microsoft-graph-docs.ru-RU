---
title: Тип перечисления safeSearchFilterType
description: Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49252525b3c6bcab6fd79a1ed7c27b3004665fe8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944798"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="b0522-103">Тип перечисления safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="b0522-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="b0522-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b0522-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0522-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0522-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0522-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b0522-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0522-107">Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="b0522-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="b0522-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b0522-108">Members</span></span>
|<span data-ttu-id="b0522-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b0522-109">Member</span></span>|<span data-ttu-id="b0522-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b0522-110">Value</span></span>|<span data-ttu-id="b0522-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0522-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0522-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="b0522-112">userDefined</span></span>|<span data-ttu-id="b0522-113">0</span><span class="sxs-lookup"><span data-stu-id="b0522-113">0</span></span>|<span data-ttu-id="b0522-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="b0522-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b0522-115">строгое</span><span class="sxs-lookup"><span data-stu-id="b0522-115">strict</span></span>|<span data-ttu-id="b0522-116">1</span><span class="sxs-lookup"><span data-stu-id="b0522-116">1</span></span>|<span data-ttu-id="b0522-117">Строгий, наибольший фильтрации содержимое для взрослых.</span><span class="sxs-lookup"><span data-stu-id="b0522-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="b0522-118">от среднего</span><span class="sxs-lookup"><span data-stu-id="b0522-118">moderate</span></span>|<span data-ttu-id="b0522-119">2</span><span class="sxs-lookup"><span data-stu-id="b0522-119">2</span></span>|<span data-ttu-id="b0522-120">От среднего фильтрации содержимое для взрослых (результаты поиска допустимый не фильтруются).</span><span class="sxs-lookup"><span data-stu-id="b0522-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





