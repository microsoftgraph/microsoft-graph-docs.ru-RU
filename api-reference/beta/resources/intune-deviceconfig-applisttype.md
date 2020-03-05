---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 96cc96d77de8b790208805dbf1a7f24a7858aa96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527083"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="1b85e-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="1b85e-103">appListType enum type</span></span>

<span data-ttu-id="1b85e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1b85e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b85e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b85e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b85e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b85e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b85e-107">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="1b85e-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="1b85e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1b85e-108">Members</span></span>
|<span data-ttu-id="1b85e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1b85e-109">Member</span></span>|<span data-ttu-id="1b85e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1b85e-110">Value</span></span>|<span data-ttu-id="1b85e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1b85e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b85e-112">нет</span><span class="sxs-lookup"><span data-stu-id="1b85e-112">none</span></span>|<span data-ttu-id="1b85e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1b85e-113">0</span></span>|<span data-ttu-id="1b85e-114">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="1b85e-114">Default value, no intent.</span></span>|
|<span data-ttu-id="1b85e-115">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="1b85e-115">appsInListCompliant</span></span>|<span data-ttu-id="1b85e-116">1 </span><span class="sxs-lookup"><span data-stu-id="1b85e-116">1</span></span>|<span data-ttu-id="1b85e-117">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="1b85e-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="1b85e-118">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="1b85e-118">appsNotInListCompliant</span></span>|<span data-ttu-id="1b85e-119">2 </span><span class="sxs-lookup"><span data-stu-id="1b85e-119">2</span></span>|<span data-ttu-id="1b85e-120">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="1b85e-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



