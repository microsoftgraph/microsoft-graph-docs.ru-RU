---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a02b8ed105206f53894ddb8d35dc24106eebebc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028604"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="beacf-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="beacf-103">appListType enum type</span></span>

> <span data-ttu-id="beacf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="beacf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beacf-105">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="beacf-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="beacf-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="beacf-106">Members</span></span>
|<span data-ttu-id="beacf-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="beacf-107">Member</span></span>|<span data-ttu-id="beacf-108">Значение</span><span class="sxs-lookup"><span data-stu-id="beacf-108">Value</span></span>|<span data-ttu-id="beacf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="beacf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beacf-110">none</span><span class="sxs-lookup"><span data-stu-id="beacf-110">none</span></span>|<span data-ttu-id="beacf-111">нуль</span><span class="sxs-lookup"><span data-stu-id="beacf-111">0</span></span>|<span data-ttu-id="beacf-112">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="beacf-112">Default value, no intent.</span></span>|
|<span data-ttu-id="beacf-113">Аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="beacf-113">appsInListCompliant</span></span>|<span data-ttu-id="beacf-114">1,1</span><span class="sxs-lookup"><span data-stu-id="beacf-114">1</span></span>|<span data-ttu-id="beacf-115">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="beacf-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="beacf-116">Аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="beacf-116">appsNotInListCompliant</span></span>|<span data-ttu-id="beacf-117">2</span><span class="sxs-lookup"><span data-stu-id="beacf-117">2</span></span>|<span data-ttu-id="beacf-118">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="beacf-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



