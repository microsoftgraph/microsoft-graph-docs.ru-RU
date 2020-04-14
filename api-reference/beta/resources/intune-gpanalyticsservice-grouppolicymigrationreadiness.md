---
title: тип перечисления Граупполицимигратионреадинесс
description: Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d05a88dd1e9aacb36968b99c2ec797c8ac3bf01f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458478"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="b4d87-103">тип перечисления Граупполицимигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="b4d87-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="b4d87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4d87-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4d87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4d87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4d87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d87-107">Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.</span><span class="sxs-lookup"><span data-stu-id="b4d87-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="b4d87-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b4d87-108">Members</span></span>
|<span data-ttu-id="b4d87-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b4d87-109">Member</span></span>|<span data-ttu-id="b4d87-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b4d87-110">Value</span></span>|<span data-ttu-id="b4d87-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b4d87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d87-112">нет</span><span class="sxs-lookup"><span data-stu-id="b4d87-112">none</span></span>|<span data-ttu-id="b4d87-113">1,1</span><span class="sxs-lookup"><span data-stu-id="b4d87-113">1</span></span>|<span data-ttu-id="b4d87-114">Нет покрытия Intune</span><span class="sxs-lookup"><span data-stu-id="b4d87-114">No Intune coverage</span></span>|
|<span data-ttu-id="b4d87-115">части</span><span class="sxs-lookup"><span data-stu-id="b4d87-115">partial</span></span>|<span data-ttu-id="b4d87-116">2</span><span class="sxs-lookup"><span data-stu-id="b4d87-116">2</span></span>|<span data-ttu-id="b4d87-117">Частичное покрытие Intune</span><span class="sxs-lookup"><span data-stu-id="b4d87-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="b4d87-118">complete</span><span class="sxs-lookup"><span data-stu-id="b4d87-118">complete</span></span>|<span data-ttu-id="b4d87-119">4</span><span class="sxs-lookup"><span data-stu-id="b4d87-119">3</span></span>|<span data-ttu-id="b4d87-120">Выполнение действия в Intune</span><span class="sxs-lookup"><span data-stu-id="b4d87-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="b4d87-121">error</span><span class="sxs-lookup"><span data-stu-id="b4d87-121">error</span></span>|<span data-ttu-id="b4d87-122">4 </span><span class="sxs-lookup"><span data-stu-id="b4d87-122">4</span></span>|<span data-ttu-id="b4d87-123">Ошибка при анализе покрытия</span><span class="sxs-lookup"><span data-stu-id="b4d87-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="b4d87-124">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="b4d87-124">notApplicable</span></span>|<span data-ttu-id="b4d87-125">5 </span><span class="sxs-lookup"><span data-stu-id="b4d87-125">5</span></span>|<span data-ttu-id="b4d87-126">Нет параметров групповой политики в объекте групповой политики</span><span class="sxs-lookup"><span data-stu-id="b4d87-126">No Group Policy settings in GPO</span></span>|



