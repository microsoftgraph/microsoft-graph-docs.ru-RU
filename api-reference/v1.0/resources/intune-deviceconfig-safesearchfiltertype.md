---
title: Тип перечисления safeSearchFilterType
description: Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным
author: tfitzmac
ms.openlocfilehash: eb0c7cfb862364ddc4703c89d19ea844ada6466d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343199"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="7a5d2-103">Тип перечисления safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="7a5d2-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="7a5d2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7a5d2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a5d2-105">Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="7a5d2-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="7a5d2-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="7a5d2-106">Members</span></span>
|<span data-ttu-id="7a5d2-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="7a5d2-107">Member</span></span>|<span data-ttu-id="7a5d2-108">Значение</span><span class="sxs-lookup"><span data-stu-id="7a5d2-108">Value</span></span>|<span data-ttu-id="7a5d2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7a5d2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a5d2-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="7a5d2-110">userDefined</span></span>|<span data-ttu-id="7a5d2-111">0</span><span class="sxs-lookup"><span data-stu-id="7a5d2-111">0</span></span>|<span data-ttu-id="7a5d2-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="7a5d2-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="7a5d2-113">строгое</span><span class="sxs-lookup"><span data-stu-id="7a5d2-113">strict</span></span>|<span data-ttu-id="7a5d2-114">1</span><span class="sxs-lookup"><span data-stu-id="7a5d2-114">1</span></span>|<span data-ttu-id="7a5d2-115">Строгий, наибольший фильтрации содержимое для взрослых.</span><span class="sxs-lookup"><span data-stu-id="7a5d2-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="7a5d2-116">от среднего</span><span class="sxs-lookup"><span data-stu-id="7a5d2-116">moderate</span></span>|<span data-ttu-id="7a5d2-117">2</span><span class="sxs-lookup"><span data-stu-id="7a5d2-117">2</span></span>|<span data-ttu-id="7a5d2-118">От среднего фильтрации содержимое для взрослых (результаты поиска допустимый не фильтруются).</span><span class="sxs-lookup"><span data-stu-id="7a5d2-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



