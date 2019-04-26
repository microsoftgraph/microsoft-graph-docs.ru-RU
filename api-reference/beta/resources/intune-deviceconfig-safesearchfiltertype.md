---
title: тип перечисления Сафесеарчфилтертипе
description: Указывает, какой уровень безопасного поиска (фильтрация содержимого для взрослых) является обязательным
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 564e641fcdc7e0d06d48666881fc3bcedfe3505c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573216"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="9c424-103">тип перечисления Сафесеарчфилтертипе</span><span class="sxs-lookup"><span data-stu-id="9c424-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="9c424-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c424-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c424-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c424-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c424-106">Указывает, какой уровень безопасного поиска (фильтрация содержимого для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="9c424-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="9c424-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9c424-107">Members</span></span>
|<span data-ttu-id="9c424-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9c424-108">Member</span></span>|<span data-ttu-id="9c424-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9c424-109">Value</span></span>|<span data-ttu-id="9c424-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9c424-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c424-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="9c424-111">userDefined</span></span>|<span data-ttu-id="9c424-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9c424-112">0</span></span>|<span data-ttu-id="9c424-113">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="9c424-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="9c424-114">жестк</span><span class="sxs-lookup"><span data-stu-id="9c424-114">strict</span></span>|<span data-ttu-id="9c424-115">1 </span><span class="sxs-lookup"><span data-stu-id="9c424-115">1</span></span>|<span data-ttu-id="9c424-116">Максимальная фильтрация с использованием содержимого для взрослых.</span><span class="sxs-lookup"><span data-stu-id="9c424-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="9c424-117">средние</span><span class="sxs-lookup"><span data-stu-id="9c424-117">moderate</span></span>|<span data-ttu-id="9c424-118">2 </span><span class="sxs-lookup"><span data-stu-id="9c424-118">2</span></span>|<span data-ttu-id="9c424-119">Умеренная фильтрация содержимого для взрослых (допустимые результаты поиска не будут фильтроваться).</span><span class="sxs-lookup"><span data-stu-id="9c424-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





