---
title: Тип перечисления safeSearchFilterType
description: Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным
ms.openlocfilehash: cf4f61e1b9e4e9f4fcfd94e6372ce517f3b735e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026200"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="ae513-103">Тип перечисления safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="ae513-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="ae513-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ae513-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae513-105">Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="ae513-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="ae513-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ae513-106">Members</span></span>
|<span data-ttu-id="ae513-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ae513-107">Member</span></span>|<span data-ttu-id="ae513-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ae513-108">Value</span></span>|<span data-ttu-id="ae513-109">Description</span><span class="sxs-lookup"><span data-stu-id="ae513-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae513-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="ae513-110">userDefined</span></span>|<span data-ttu-id="ae513-111">0</span><span class="sxs-lookup"><span data-stu-id="ae513-111">0</span></span>|<span data-ttu-id="ae513-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="ae513-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ae513-113">строгое</span><span class="sxs-lookup"><span data-stu-id="ae513-113">strict</span></span>|<span data-ttu-id="ae513-114">1</span><span class="sxs-lookup"><span data-stu-id="ae513-114">1</span></span>|<span data-ttu-id="ae513-115">Строгий, наибольший фильтрации содержимое для взрослых.</span><span class="sxs-lookup"><span data-stu-id="ae513-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="ae513-116">от среднего</span><span class="sxs-lookup"><span data-stu-id="ae513-116">moderate</span></span>|<span data-ttu-id="ae513-117">2</span><span class="sxs-lookup"><span data-stu-id="ae513-117">2</span></span>|<span data-ttu-id="ae513-118">От среднего фильтрации содержимое для взрослых (результаты поиска допустимый не фильтруются).</span><span class="sxs-lookup"><span data-stu-id="ae513-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



