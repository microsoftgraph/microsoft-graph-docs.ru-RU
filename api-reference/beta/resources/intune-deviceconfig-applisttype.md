---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dca4f368f63296ed2fe751080fcce9c51549b280
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011493"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="88736-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="88736-103">appListType enum type</span></span>

> <span data-ttu-id="88736-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88736-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88736-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88736-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88736-106">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="88736-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="88736-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="88736-107">Members</span></span>
|<span data-ttu-id="88736-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="88736-108">Member</span></span>|<span data-ttu-id="88736-109">Значение</span><span class="sxs-lookup"><span data-stu-id="88736-109">Value</span></span>|<span data-ttu-id="88736-110">Описание</span><span class="sxs-lookup"><span data-stu-id="88736-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88736-111">none</span><span class="sxs-lookup"><span data-stu-id="88736-111">none</span></span>|<span data-ttu-id="88736-112">нуль</span><span class="sxs-lookup"><span data-stu-id="88736-112">0</span></span>|<span data-ttu-id="88736-113">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="88736-113">Default value, no intent.</span></span>|
|<span data-ttu-id="88736-114">Аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="88736-114">appsInListCompliant</span></span>|<span data-ttu-id="88736-115">1,1</span><span class="sxs-lookup"><span data-stu-id="88736-115">1</span></span>|<span data-ttu-id="88736-116">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="88736-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="88736-117">Аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="88736-117">appsNotInListCompliant</span></span>|<span data-ttu-id="88736-118">2</span><span class="sxs-lookup"><span data-stu-id="88736-118">2</span></span>|<span data-ttu-id="88736-119">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="88736-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





