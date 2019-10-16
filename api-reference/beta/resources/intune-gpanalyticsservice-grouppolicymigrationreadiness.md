---
title: тип перечисления Граупполицимигратионреадинесс
description: Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb87c31bfe92a8845953e6e2a264ec60c9a3d863
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539108"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="2fade-103">тип перечисления Граупполицимигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="2fade-103">groupPolicyMigrationReadiness enum type</span></span>

> <span data-ttu-id="2fade-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fade-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fade-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fade-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fade-106">Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.</span><span class="sxs-lookup"><span data-stu-id="2fade-106">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="2fade-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2fade-107">Members</span></span>
|<span data-ttu-id="2fade-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2fade-108">Member</span></span>|<span data-ttu-id="2fade-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2fade-109">Value</span></span>|<span data-ttu-id="2fade-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2fade-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fade-111">none</span><span class="sxs-lookup"><span data-stu-id="2fade-111">none</span></span>|<span data-ttu-id="2fade-112">1,1</span><span class="sxs-lookup"><span data-stu-id="2fade-112">1</span></span>|<span data-ttu-id="2fade-113">Нет покрытия Intune</span><span class="sxs-lookup"><span data-stu-id="2fade-113">No Intune coverage</span></span>|
|<span data-ttu-id="2fade-114">части</span><span class="sxs-lookup"><span data-stu-id="2fade-114">partial</span></span>|<span data-ttu-id="2fade-115">2</span><span class="sxs-lookup"><span data-stu-id="2fade-115">2</span></span>|<span data-ttu-id="2fade-116">Частичное покрытие Intune</span><span class="sxs-lookup"><span data-stu-id="2fade-116">Partial Intune coverage</span></span>|
|<span data-ttu-id="2fade-117">complete</span><span class="sxs-lookup"><span data-stu-id="2fade-117">complete</span></span>|<span data-ttu-id="2fade-118">4</span><span class="sxs-lookup"><span data-stu-id="2fade-118">3</span></span>|<span data-ttu-id="2fade-119">Выполнение действия в Intune</span><span class="sxs-lookup"><span data-stu-id="2fade-119">Complete Intune coverage</span></span>|
|<span data-ttu-id="2fade-120">error</span><span class="sxs-lookup"><span data-stu-id="2fade-120">error</span></span>|<span data-ttu-id="2fade-121">4 </span><span class="sxs-lookup"><span data-stu-id="2fade-121">4</span></span>|<span data-ttu-id="2fade-122">Ошибка при анализе покрытия</span><span class="sxs-lookup"><span data-stu-id="2fade-122">Error when analyzing coverage</span></span>|
|<span data-ttu-id="2fade-123">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="2fade-123">notApplicable</span></span>|<span data-ttu-id="2fade-124">5 </span><span class="sxs-lookup"><span data-stu-id="2fade-124">5</span></span>|<span data-ttu-id="2fade-125">Нет параметров групповой политики в объекте групповой политики</span><span class="sxs-lookup"><span data-stu-id="2fade-125">No Group Policy settings in GPO</span></span>|



