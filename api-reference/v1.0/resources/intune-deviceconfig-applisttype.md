---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575102"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="5316e-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="5316e-103">appListType enum type</span></span>

> <span data-ttu-id="5316e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5316e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5316e-105">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="5316e-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="5316e-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="5316e-106">Members</span></span>
|<span data-ttu-id="5316e-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="5316e-107">Member</span></span>|<span data-ttu-id="5316e-108">Значение</span><span class="sxs-lookup"><span data-stu-id="5316e-108">Value</span></span>|<span data-ttu-id="5316e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5316e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5316e-110">Нет</span><span class="sxs-lookup"><span data-stu-id="5316e-110">none</span></span>|<span data-ttu-id="5316e-111">нуль</span><span class="sxs-lookup"><span data-stu-id="5316e-111">0</span></span>|<span data-ttu-id="5316e-112">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="5316e-112">Default value, no intent.</span></span>|
|<span data-ttu-id="5316e-113">Аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="5316e-113">appsInListCompliant</span></span>|<span data-ttu-id="5316e-114">1 </span><span class="sxs-lookup"><span data-stu-id="5316e-114">1</span></span>|<span data-ttu-id="5316e-115">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="5316e-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="5316e-116">Аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="5316e-116">appsNotInListCompliant</span></span>|<span data-ttu-id="5316e-117">2 </span><span class="sxs-lookup"><span data-stu-id="5316e-117">2</span></span>|<span data-ttu-id="5316e-118">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="5316e-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



