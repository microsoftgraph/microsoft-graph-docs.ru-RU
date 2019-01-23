---
title: Тип перечисления safeSearchFilterType
description: Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4493c71b48a0f5ff4b0c48307504087c722393e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403485"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="045e5-103">Тип перечисления safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="045e5-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="045e5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="045e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="045e5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="045e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="045e5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="045e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="045e5-107">Указывает, какой уровень безопасного поиска (фильтрация содержимое для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="045e5-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="045e5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="045e5-108">Members</span></span>
|<span data-ttu-id="045e5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="045e5-109">Member</span></span>|<span data-ttu-id="045e5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="045e5-110">Value</span></span>|<span data-ttu-id="045e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="045e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="045e5-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="045e5-112">userDefined</span></span>|<span data-ttu-id="045e5-113">0</span><span class="sxs-lookup"><span data-stu-id="045e5-113">0</span></span>|<span data-ttu-id="045e5-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="045e5-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="045e5-115">строгое</span><span class="sxs-lookup"><span data-stu-id="045e5-115">strict</span></span>|<span data-ttu-id="045e5-116">1</span><span class="sxs-lookup"><span data-stu-id="045e5-116">1</span></span>|<span data-ttu-id="045e5-117">Строгий, наибольший фильтрации содержимое для взрослых.</span><span class="sxs-lookup"><span data-stu-id="045e5-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="045e5-118">от среднего</span><span class="sxs-lookup"><span data-stu-id="045e5-118">moderate</span></span>|<span data-ttu-id="045e5-119">2</span><span class="sxs-lookup"><span data-stu-id="045e5-119">2</span></span>|<span data-ttu-id="045e5-120">От среднего фильтрации содержимое для взрослых (результаты поиска допустимый не фильтруются).</span><span class="sxs-lookup"><span data-stu-id="045e5-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




