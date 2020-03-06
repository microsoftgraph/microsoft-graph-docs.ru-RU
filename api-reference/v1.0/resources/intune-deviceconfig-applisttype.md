---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ead624878dafd1d2edd1aca27d689da5af57de8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532625"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="3b404-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="3b404-103">appListType enum type</span></span>

<span data-ttu-id="3b404-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b404-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b404-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b404-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b404-106">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b404-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="3b404-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3b404-107">Members</span></span>
|<span data-ttu-id="3b404-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3b404-108">Member</span></span>|<span data-ttu-id="3b404-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3b404-109">Value</span></span>|<span data-ttu-id="3b404-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b404-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b404-111">нет</span><span class="sxs-lookup"><span data-stu-id="3b404-111">none</span></span>|<span data-ttu-id="3b404-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3b404-112">0</span></span>|<span data-ttu-id="3b404-113">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="3b404-113">Default value, no intent.</span></span>|
|<span data-ttu-id="3b404-114">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="3b404-114">appsInListCompliant</span></span>|<span data-ttu-id="3b404-115">1 </span><span class="sxs-lookup"><span data-stu-id="3b404-115">1</span></span>|<span data-ttu-id="3b404-116">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="3b404-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="3b404-117">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="3b404-117">appsNotInListCompliant</span></span>|<span data-ttu-id="3b404-118">2 </span><span class="sxs-lookup"><span data-stu-id="3b404-118">2</span></span>|<span data-ttu-id="3b404-119">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="3b404-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




