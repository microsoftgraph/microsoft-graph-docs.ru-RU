---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254326"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="5e38c-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="5e38c-103">appListType enum type</span></span>

> <span data-ttu-id="5e38c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e38c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e38c-105">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="5e38c-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="5e38c-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="5e38c-106">Members</span></span>
|<span data-ttu-id="5e38c-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="5e38c-107">Member</span></span>|<span data-ttu-id="5e38c-108">Значение</span><span class="sxs-lookup"><span data-stu-id="5e38c-108">Value</span></span>|<span data-ttu-id="5e38c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5e38c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e38c-110">Нет</span><span class="sxs-lookup"><span data-stu-id="5e38c-110">none</span></span>|<span data-ttu-id="5e38c-111">нуль</span><span class="sxs-lookup"><span data-stu-id="5e38c-111">0</span></span>|<span data-ttu-id="5e38c-112">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="5e38c-112">Default value, no intent.</span></span>|
|<span data-ttu-id="5e38c-113">Аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="5e38c-113">appsInListCompliant</span></span>|<span data-ttu-id="5e38c-114">1,1</span><span class="sxs-lookup"><span data-stu-id="5e38c-114">1</span></span>|<span data-ttu-id="5e38c-115">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="5e38c-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="5e38c-116">Аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="5e38c-116">appsNotInListCompliant</span></span>|<span data-ttu-id="5e38c-117">2</span><span class="sxs-lookup"><span data-stu-id="5e38c-117">2</span></span>|<span data-ttu-id="5e38c-118">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="5e38c-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



