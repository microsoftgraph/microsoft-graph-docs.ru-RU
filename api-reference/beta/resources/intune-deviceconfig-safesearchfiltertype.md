---
title: тип перечисления Сафесеарчфилтертипе
description: Указывает, какой уровень безопасного поиска (фильтрация содержимого для взрослых) является обязательным
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 92cad118957ea383b886cccc8fb29066e8b2fd20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529438"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="6c694-103">тип перечисления Сафесеарчфилтертипе</span><span class="sxs-lookup"><span data-stu-id="6c694-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="6c694-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6c694-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c694-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c694-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c694-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c694-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c694-107">Указывает, какой уровень безопасного поиска (фильтрация содержимого для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="6c694-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="6c694-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6c694-108">Members</span></span>
|<span data-ttu-id="6c694-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6c694-109">Member</span></span>|<span data-ttu-id="6c694-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6c694-110">Value</span></span>|<span data-ttu-id="6c694-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6c694-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c694-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="6c694-112">userDefined</span></span>|<span data-ttu-id="6c694-113">нуль</span><span class="sxs-lookup"><span data-stu-id="6c694-113">0</span></span>|<span data-ttu-id="6c694-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="6c694-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="6c694-115">жестк</span><span class="sxs-lookup"><span data-stu-id="6c694-115">strict</span></span>|<span data-ttu-id="6c694-116">1 </span><span class="sxs-lookup"><span data-stu-id="6c694-116">1</span></span>|<span data-ttu-id="6c694-117">Максимальная фильтрация с использованием содержимого для взрослых.</span><span class="sxs-lookup"><span data-stu-id="6c694-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="6c694-118">средние</span><span class="sxs-lookup"><span data-stu-id="6c694-118">moderate</span></span>|<span data-ttu-id="6c694-119">2 </span><span class="sxs-lookup"><span data-stu-id="6c694-119">2</span></span>|<span data-ttu-id="6c694-120">Умеренная фильтрация содержимого для взрослых (допустимые результаты поиска не будут фильтроваться).</span><span class="sxs-lookup"><span data-stu-id="6c694-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



