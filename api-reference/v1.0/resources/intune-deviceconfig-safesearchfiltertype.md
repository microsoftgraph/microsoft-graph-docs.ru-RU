---
title: Тип перечисления safeSearchFilterType
description: Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28aea918c35bb9d90f514e4a8838f219c212405b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830858"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="ebb36-103">Тип перечисления safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="ebb36-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="ebb36-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ebb36-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebb36-105">Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="ebb36-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="ebb36-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ebb36-106">Members</span></span>
|<span data-ttu-id="ebb36-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ebb36-107">Member</span></span>|<span data-ttu-id="ebb36-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ebb36-108">Value</span></span>|<span data-ttu-id="ebb36-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb36-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb36-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="ebb36-110">userDefined</span></span>|<span data-ttu-id="ebb36-111">0</span><span class="sxs-lookup"><span data-stu-id="ebb36-111">0</span></span>|<span data-ttu-id="ebb36-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="ebb36-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ebb36-113">строгое</span><span class="sxs-lookup"><span data-stu-id="ebb36-113">strict</span></span>|<span data-ttu-id="ebb36-114">1</span><span class="sxs-lookup"><span data-stu-id="ebb36-114">1</span></span>|<span data-ttu-id="ebb36-115">Строгий, наибольший фильтрации содержимое для взрослых.</span><span class="sxs-lookup"><span data-stu-id="ebb36-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="ebb36-116">от среднего</span><span class="sxs-lookup"><span data-stu-id="ebb36-116">moderate</span></span>|<span data-ttu-id="ebb36-117">2</span><span class="sxs-lookup"><span data-stu-id="ebb36-117">2</span></span>|<span data-ttu-id="ebb36-118">От среднего фильтрации содержимое для взрослых (результаты поиска допустимый не фильтруются).</span><span class="sxs-lookup"><span data-stu-id="ebb36-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



