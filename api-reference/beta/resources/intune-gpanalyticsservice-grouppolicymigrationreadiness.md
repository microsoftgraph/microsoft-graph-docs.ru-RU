---
title: тип перечисления Граупполицимигратионреадинесс
description: Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 15e7d0a626934f8f6d17aebf6eff9aff8c537dbd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031230"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="f51ec-103">тип перечисления Граупполицимигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="f51ec-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="f51ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f51ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f51ec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f51ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f51ec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f51ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f51ec-107">Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.</span><span class="sxs-lookup"><span data-stu-id="f51ec-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="f51ec-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f51ec-108">Members</span></span>
|<span data-ttu-id="f51ec-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f51ec-109">Member</span></span>|<span data-ttu-id="f51ec-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f51ec-110">Value</span></span>|<span data-ttu-id="f51ec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f51ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f51ec-112">Нет</span><span class="sxs-lookup"><span data-stu-id="f51ec-112">none</span></span>|<span data-ttu-id="f51ec-113">1 </span><span class="sxs-lookup"><span data-stu-id="f51ec-113">1</span></span>|<span data-ttu-id="f51ec-114">Нет покрытия Intune</span><span class="sxs-lookup"><span data-stu-id="f51ec-114">No Intune coverage</span></span>|
|<span data-ttu-id="f51ec-115">части</span><span class="sxs-lookup"><span data-stu-id="f51ec-115">partial</span></span>|<span data-ttu-id="f51ec-116">2 </span><span class="sxs-lookup"><span data-stu-id="f51ec-116">2</span></span>|<span data-ttu-id="f51ec-117">Частичное покрытие Intune</span><span class="sxs-lookup"><span data-stu-id="f51ec-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="f51ec-118">complete</span><span class="sxs-lookup"><span data-stu-id="f51ec-118">complete</span></span>|<span data-ttu-id="f51ec-119">4</span><span class="sxs-lookup"><span data-stu-id="f51ec-119">3</span></span>|<span data-ttu-id="f51ec-120">Выполнение действия в Intune</span><span class="sxs-lookup"><span data-stu-id="f51ec-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="f51ec-121">error</span><span class="sxs-lookup"><span data-stu-id="f51ec-121">error</span></span>|<span data-ttu-id="f51ec-122">4 </span><span class="sxs-lookup"><span data-stu-id="f51ec-122">4</span></span>|<span data-ttu-id="f51ec-123">Ошибка при анализе покрытия</span><span class="sxs-lookup"><span data-stu-id="f51ec-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="f51ec-124">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="f51ec-124">notApplicable</span></span>|<span data-ttu-id="f51ec-125">5 </span><span class="sxs-lookup"><span data-stu-id="f51ec-125">5</span></span>|<span data-ttu-id="f51ec-126">Нет параметров групповой политики в объекте групповой политики</span><span class="sxs-lookup"><span data-stu-id="f51ec-126">No Group Policy settings in GPO</span></span>|






