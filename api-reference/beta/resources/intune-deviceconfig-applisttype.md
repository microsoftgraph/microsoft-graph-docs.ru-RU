---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a05fc37f692d58a4d5d434037fd9d1ebe09ecaa9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798728"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="8019f-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="8019f-103">appListType enum type</span></span>

> <span data-ttu-id="8019f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8019f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8019f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8019f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8019f-106">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="8019f-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="8019f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8019f-107">Members</span></span>
|<span data-ttu-id="8019f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8019f-108">Member</span></span>|<span data-ttu-id="8019f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8019f-109">Value</span></span>|<span data-ttu-id="8019f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8019f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8019f-111">нет</span><span class="sxs-lookup"><span data-stu-id="8019f-111">none</span></span>|<span data-ttu-id="8019f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8019f-112">0</span></span>|<span data-ttu-id="8019f-113">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="8019f-113">Default value, no intent.</span></span>|
|<span data-ttu-id="8019f-114">Аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="8019f-114">appsInListCompliant</span></span>|<span data-ttu-id="8019f-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8019f-115">1</span></span>|<span data-ttu-id="8019f-116">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="8019f-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="8019f-117">Аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="8019f-117">appsNotInListCompliant</span></span>|<span data-ttu-id="8019f-118">2</span><span class="sxs-lookup"><span data-stu-id="8019f-118">2</span></span>|<span data-ttu-id="8019f-119">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="8019f-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





