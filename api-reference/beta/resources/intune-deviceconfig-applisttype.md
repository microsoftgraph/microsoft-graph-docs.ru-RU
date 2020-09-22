---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 49ef93ede45fd784f4b0b9bc52010dce80fa2eb1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075968"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="6f977-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="6f977-103">appListType enum type</span></span>

<span data-ttu-id="6f977-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f977-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f977-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f977-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f977-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f977-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f977-107">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="6f977-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="6f977-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6f977-108">Members</span></span>
|<span data-ttu-id="6f977-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6f977-109">Member</span></span>|<span data-ttu-id="6f977-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6f977-110">Value</span></span>|<span data-ttu-id="6f977-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6f977-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f977-112">Нет</span><span class="sxs-lookup"><span data-stu-id="6f977-112">none</span></span>|<span data-ttu-id="6f977-113">нуль</span><span class="sxs-lookup"><span data-stu-id="6f977-113">0</span></span>|<span data-ttu-id="6f977-114">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="6f977-114">Default value, no intent.</span></span>|
|<span data-ttu-id="6f977-115">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="6f977-115">appsInListCompliant</span></span>|<span data-ttu-id="6f977-116">1 </span><span class="sxs-lookup"><span data-stu-id="6f977-116">1</span></span>|<span data-ttu-id="6f977-117">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="6f977-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="6f977-118">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="6f977-118">appsNotInListCompliant</span></span>|<span data-ttu-id="6f977-119">2 </span><span class="sxs-lookup"><span data-stu-id="6f977-119">2</span></span>|<span data-ttu-id="6f977-120">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="6f977-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|






