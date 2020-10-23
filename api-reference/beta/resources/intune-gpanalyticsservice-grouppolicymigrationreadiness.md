---
title: тип перечисления Граупполицимигратионреадинесс
description: Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d860844de50c58deace7f10821ca0b1a4591d00b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722825"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="e7d48-103">тип перечисления Граупполицимигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="e7d48-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="e7d48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7d48-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7d48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7d48-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7d48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7d48-107">Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.</span><span class="sxs-lookup"><span data-stu-id="e7d48-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="e7d48-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e7d48-108">Members</span></span>
|<span data-ttu-id="e7d48-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e7d48-109">Member</span></span>|<span data-ttu-id="e7d48-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e7d48-110">Value</span></span>|<span data-ttu-id="e7d48-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e7d48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d48-112">none</span><span class="sxs-lookup"><span data-stu-id="e7d48-112">none</span></span>|<span data-ttu-id="e7d48-113">1,1</span><span class="sxs-lookup"><span data-stu-id="e7d48-113">1</span></span>|<span data-ttu-id="e7d48-114">Нет покрытия Intune</span><span class="sxs-lookup"><span data-stu-id="e7d48-114">No Intune coverage</span></span>|
|<span data-ttu-id="e7d48-115">части</span><span class="sxs-lookup"><span data-stu-id="e7d48-115">partial</span></span>|<span data-ttu-id="e7d48-116">2</span><span class="sxs-lookup"><span data-stu-id="e7d48-116">2</span></span>|<span data-ttu-id="e7d48-117">Частичное покрытие Intune</span><span class="sxs-lookup"><span data-stu-id="e7d48-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="e7d48-118">complete</span><span class="sxs-lookup"><span data-stu-id="e7d48-118">complete</span></span>|<span data-ttu-id="e7d48-119">4</span><span class="sxs-lookup"><span data-stu-id="e7d48-119">3</span></span>|<span data-ttu-id="e7d48-120">Выполнение действия в Intune</span><span class="sxs-lookup"><span data-stu-id="e7d48-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="e7d48-121">error</span><span class="sxs-lookup"><span data-stu-id="e7d48-121">error</span></span>|<span data-ttu-id="e7d48-122">4 </span><span class="sxs-lookup"><span data-stu-id="e7d48-122">4</span></span>|<span data-ttu-id="e7d48-123">Ошибка при анализе покрытия</span><span class="sxs-lookup"><span data-stu-id="e7d48-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="e7d48-124">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="e7d48-124">notApplicable</span></span>|<span data-ttu-id="e7d48-125">5 </span><span class="sxs-lookup"><span data-stu-id="e7d48-125">5</span></span>|<span data-ttu-id="e7d48-126">Нет параметров групповой политики в объекте групповой политики</span><span class="sxs-lookup"><span data-stu-id="e7d48-126">No Group Policy settings in GPO</span></span>|





