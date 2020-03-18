---
title: тип перечисления Граупполицимигратионреадинесс
description: Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efd579adb3c3408eda9b87ffb7f48e98c836065f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783174"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="bd5b9-103">тип перечисления Граупполицимигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="bd5b9-103">groupPolicyMigrationReadiness enum type</span></span>

> <span data-ttu-id="bd5b9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd5b9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd5b9-106">Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-106">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="bd5b9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bd5b9-107">Members</span></span>
|<span data-ttu-id="bd5b9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bd5b9-108">Member</span></span>|<span data-ttu-id="bd5b9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bd5b9-109">Value</span></span>|<span data-ttu-id="bd5b9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd5b9-111">none</span><span class="sxs-lookup"><span data-stu-id="bd5b9-111">none</span></span>|<span data-ttu-id="bd5b9-112">1,1</span><span class="sxs-lookup"><span data-stu-id="bd5b9-112">1</span></span>|<span data-ttu-id="bd5b9-113">Нет покрытия Intune</span><span class="sxs-lookup"><span data-stu-id="bd5b9-113">No Intune coverage</span></span>|
|<span data-ttu-id="bd5b9-114">части</span><span class="sxs-lookup"><span data-stu-id="bd5b9-114">partial</span></span>|<span data-ttu-id="bd5b9-115">2</span><span class="sxs-lookup"><span data-stu-id="bd5b9-115">2</span></span>|<span data-ttu-id="bd5b9-116">Частичное покрытие Intune</span><span class="sxs-lookup"><span data-stu-id="bd5b9-116">Partial Intune coverage</span></span>|
|<span data-ttu-id="bd5b9-117">complete</span><span class="sxs-lookup"><span data-stu-id="bd5b9-117">complete</span></span>|<span data-ttu-id="bd5b9-118">4</span><span class="sxs-lookup"><span data-stu-id="bd5b9-118">3</span></span>|<span data-ttu-id="bd5b9-119">Выполнение действия в Intune</span><span class="sxs-lookup"><span data-stu-id="bd5b9-119">Complete Intune coverage</span></span>|
|<span data-ttu-id="bd5b9-120">error</span><span class="sxs-lookup"><span data-stu-id="bd5b9-120">error</span></span>|<span data-ttu-id="bd5b9-121">4 </span><span class="sxs-lookup"><span data-stu-id="bd5b9-121">4</span></span>|<span data-ttu-id="bd5b9-122">Ошибка при анализе покрытия</span><span class="sxs-lookup"><span data-stu-id="bd5b9-122">Error when analyzing coverage</span></span>|
|<span data-ttu-id="bd5b9-123">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="bd5b9-123">notApplicable</span></span>|<span data-ttu-id="bd5b9-124">5 </span><span class="sxs-lookup"><span data-stu-id="bd5b9-124">5</span></span>|<span data-ttu-id="bd5b9-125">Нет параметров групповой политики в объекте групповой политики</span><span class="sxs-lookup"><span data-stu-id="bd5b9-125">No Group Policy settings in GPO</span></span>|



