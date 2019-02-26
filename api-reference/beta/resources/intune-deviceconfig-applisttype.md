---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b7d11107ca3ea2b698e28cd288f163ec190b0a6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172676"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="cc915-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="cc915-103">appListType enum type</span></span>

> <span data-ttu-id="cc915-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc915-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc915-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc915-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc915-106">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="cc915-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="cc915-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cc915-107">Members</span></span>
|<span data-ttu-id="cc915-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cc915-108">Member</span></span>|<span data-ttu-id="cc915-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cc915-109">Value</span></span>|<span data-ttu-id="cc915-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cc915-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc915-111">Нет</span><span class="sxs-lookup"><span data-stu-id="cc915-111">none</span></span>|<span data-ttu-id="cc915-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cc915-112">0</span></span>|<span data-ttu-id="cc915-113">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="cc915-113">Default value, no intent.</span></span>|
|<span data-ttu-id="cc915-114">Аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="cc915-114">appsInListCompliant</span></span>|<span data-ttu-id="cc915-115">1,1</span><span class="sxs-lookup"><span data-stu-id="cc915-115">1</span></span>|<span data-ttu-id="cc915-116">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="cc915-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="cc915-117">Аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="cc915-117">appsNotInListCompliant</span></span>|<span data-ttu-id="cc915-118">2</span><span class="sxs-lookup"><span data-stu-id="cc915-118">2</span></span>|<span data-ttu-id="cc915-119">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="cc915-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




