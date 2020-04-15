---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a372f2f160a4a08a1c9f1c3e4276ea10344daff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449157"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="bc0a4-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="bc0a4-103">appListType enum type</span></span>

<span data-ttu-id="bc0a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc0a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc0a4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc0a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc0a4-106">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="bc0a4-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="bc0a4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bc0a4-107">Members</span></span>
|<span data-ttu-id="bc0a4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bc0a4-108">Member</span></span>|<span data-ttu-id="bc0a4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bc0a4-109">Value</span></span>|<span data-ttu-id="bc0a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc0a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc0a4-111">нет</span><span class="sxs-lookup"><span data-stu-id="bc0a4-111">none</span></span>|<span data-ttu-id="bc0a4-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bc0a4-112">0</span></span>|<span data-ttu-id="bc0a4-113">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="bc0a4-113">Default value, no intent.</span></span>|
|<span data-ttu-id="bc0a4-114">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="bc0a4-114">appsInListCompliant</span></span>|<span data-ttu-id="bc0a4-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bc0a4-115">1</span></span>|<span data-ttu-id="bc0a4-116">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="bc0a4-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="bc0a4-117">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="bc0a4-117">appsNotInListCompliant</span></span>|<span data-ttu-id="bc0a4-118">2</span><span class="sxs-lookup"><span data-stu-id="bc0a4-118">2</span></span>|<span data-ttu-id="bc0a4-119">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="bc0a4-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|







