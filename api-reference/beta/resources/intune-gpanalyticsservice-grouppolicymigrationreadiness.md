---
title: тип перечисления Граупполицимигратионреадинесс
description: Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6b2ec4f8363f6ad68cd34a77287502eaadf2d52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524485"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="ef982-103">тип перечисления Граупполицимигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="ef982-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="ef982-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ef982-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef982-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef982-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef982-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef982-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef982-107">Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.</span><span class="sxs-lookup"><span data-stu-id="ef982-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="ef982-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ef982-108">Members</span></span>
|<span data-ttu-id="ef982-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ef982-109">Member</span></span>|<span data-ttu-id="ef982-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ef982-110">Value</span></span>|<span data-ttu-id="ef982-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ef982-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef982-112">нет</span><span class="sxs-lookup"><span data-stu-id="ef982-112">none</span></span>|<span data-ttu-id="ef982-113">1 </span><span class="sxs-lookup"><span data-stu-id="ef982-113">1</span></span>|<span data-ttu-id="ef982-114">Нет покрытия Intune</span><span class="sxs-lookup"><span data-stu-id="ef982-114">No Intune coverage</span></span>|
|<span data-ttu-id="ef982-115">части</span><span class="sxs-lookup"><span data-stu-id="ef982-115">partial</span></span>|<span data-ttu-id="ef982-116">2 </span><span class="sxs-lookup"><span data-stu-id="ef982-116">2</span></span>|<span data-ttu-id="ef982-117">Частичное покрытие Intune</span><span class="sxs-lookup"><span data-stu-id="ef982-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="ef982-118">complete</span><span class="sxs-lookup"><span data-stu-id="ef982-118">complete</span></span>|<span data-ttu-id="ef982-119">3 </span><span class="sxs-lookup"><span data-stu-id="ef982-119">3</span></span>|<span data-ttu-id="ef982-120">Выполнение действия в Intune</span><span class="sxs-lookup"><span data-stu-id="ef982-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="ef982-121">error</span><span class="sxs-lookup"><span data-stu-id="ef982-121">error</span></span>|<span data-ttu-id="ef982-122">4 </span><span class="sxs-lookup"><span data-stu-id="ef982-122">4</span></span>|<span data-ttu-id="ef982-123">Ошибка при анализе покрытия</span><span class="sxs-lookup"><span data-stu-id="ef982-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="ef982-124">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="ef982-124">notApplicable</span></span>|<span data-ttu-id="ef982-125">5 </span><span class="sxs-lookup"><span data-stu-id="ef982-125">5</span></span>|<span data-ttu-id="ef982-126">Нет параметров групповой политики в объекте групповой политики</span><span class="sxs-lookup"><span data-stu-id="ef982-126">No Group Policy settings in GPO</span></span>|



