---
title: тип перечисления Сафесеарчфилтертипе
description: Указывает, какой уровень безопасного поиска (фильтрация содержимого для взрослых) является обязательным
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 54beae59c3341605b8b4a7c3f482c8d98d31851b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293901"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="fe3cb-103">тип перечисления Сафесеарчфилтертипе</span><span class="sxs-lookup"><span data-stu-id="fe3cb-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="fe3cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe3cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe3cb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe3cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe3cb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe3cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe3cb-107">Указывает, какой уровень безопасного поиска (фильтрация содержимого для взрослых) является обязательным</span><span class="sxs-lookup"><span data-stu-id="fe3cb-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="fe3cb-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fe3cb-108">Members</span></span>
|<span data-ttu-id="fe3cb-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fe3cb-109">Member</span></span>|<span data-ttu-id="fe3cb-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fe3cb-110">Value</span></span>|<span data-ttu-id="fe3cb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe3cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe3cb-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="fe3cb-112">userDefined</span></span>|<span data-ttu-id="fe3cb-113">нуль</span><span class="sxs-lookup"><span data-stu-id="fe3cb-113">0</span></span>|<span data-ttu-id="fe3cb-114">Пользователь определен, значение по умолчанию, без намерения.</span><span class="sxs-lookup"><span data-stu-id="fe3cb-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="fe3cb-115">жестк</span><span class="sxs-lookup"><span data-stu-id="fe3cb-115">strict</span></span>|<span data-ttu-id="fe3cb-116">1,1</span><span class="sxs-lookup"><span data-stu-id="fe3cb-116">1</span></span>|<span data-ttu-id="fe3cb-117">Максимальная фильтрация с использованием содержимого для взрослых.</span><span class="sxs-lookup"><span data-stu-id="fe3cb-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="fe3cb-118">средние</span><span class="sxs-lookup"><span data-stu-id="fe3cb-118">moderate</span></span>|<span data-ttu-id="fe3cb-119">2</span><span class="sxs-lookup"><span data-stu-id="fe3cb-119">2</span></span>|<span data-ttu-id="fe3cb-120">Умеренная фильтрация содержимого для взрослых (допустимые результаты поиска не будут фильтроваться).</span><span class="sxs-lookup"><span data-stu-id="fe3cb-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




