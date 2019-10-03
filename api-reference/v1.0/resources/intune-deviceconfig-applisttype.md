---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c46f059721727e8752df6f7b0ad99a48c3104d64
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366729"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="d3ced-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="d3ced-103">appListType enum type</span></span>

> <span data-ttu-id="d3ced-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3ced-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3ced-105">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="d3ced-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="d3ced-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="d3ced-106">Members</span></span>
|<span data-ttu-id="d3ced-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="d3ced-107">Member</span></span>|<span data-ttu-id="d3ced-108">Значение</span><span class="sxs-lookup"><span data-stu-id="d3ced-108">Value</span></span>|<span data-ttu-id="d3ced-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d3ced-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3ced-110">none</span><span class="sxs-lookup"><span data-stu-id="d3ced-110">none</span></span>|<span data-ttu-id="d3ced-111">нуль</span><span class="sxs-lookup"><span data-stu-id="d3ced-111">0</span></span>|<span data-ttu-id="d3ced-112">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="d3ced-112">Default value, no intent.</span></span>|
|<span data-ttu-id="d3ced-113">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="d3ced-113">appsInListCompliant</span></span>|<span data-ttu-id="d3ced-114">1,1</span><span class="sxs-lookup"><span data-stu-id="d3ced-114">1</span></span>|<span data-ttu-id="d3ced-115">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="d3ced-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="d3ced-116">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="d3ced-116">appsNotInListCompliant</span></span>|<span data-ttu-id="d3ced-117">2</span><span class="sxs-lookup"><span data-stu-id="d3ced-117">2</span></span>|<span data-ttu-id="d3ced-118">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="d3ced-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




