---
title: тип перечисления Граупполицимигратионреадинесс
description: Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 30d223eb59d092b9411388b93226d48165a4e703
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298766"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="dd54c-103">тип перечисления Граупполицимигратионреадинесс</span><span class="sxs-lookup"><span data-stu-id="dd54c-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="dd54c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd54c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd54c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd54c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd54c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd54c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd54c-107">Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.</span><span class="sxs-lookup"><span data-stu-id="dd54c-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="dd54c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dd54c-108">Members</span></span>
|<span data-ttu-id="dd54c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dd54c-109">Member</span></span>|<span data-ttu-id="dd54c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dd54c-110">Value</span></span>|<span data-ttu-id="dd54c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dd54c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd54c-112">Нет</span><span class="sxs-lookup"><span data-stu-id="dd54c-112">none</span></span>|<span data-ttu-id="dd54c-113">1,1</span><span class="sxs-lookup"><span data-stu-id="dd54c-113">1</span></span>|<span data-ttu-id="dd54c-114">Нет покрытия Intune</span><span class="sxs-lookup"><span data-stu-id="dd54c-114">No Intune coverage</span></span>|
|<span data-ttu-id="dd54c-115">части</span><span class="sxs-lookup"><span data-stu-id="dd54c-115">partial</span></span>|<span data-ttu-id="dd54c-116">2</span><span class="sxs-lookup"><span data-stu-id="dd54c-116">2</span></span>|<span data-ttu-id="dd54c-117">Частичное покрытие Intune</span><span class="sxs-lookup"><span data-stu-id="dd54c-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="dd54c-118">complete</span><span class="sxs-lookup"><span data-stu-id="dd54c-118">complete</span></span>|<span data-ttu-id="dd54c-119">4</span><span class="sxs-lookup"><span data-stu-id="dd54c-119">3</span></span>|<span data-ttu-id="dd54c-120">Выполнение действия в Intune</span><span class="sxs-lookup"><span data-stu-id="dd54c-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="dd54c-121">error</span><span class="sxs-lookup"><span data-stu-id="dd54c-121">error</span></span>|<span data-ttu-id="dd54c-122">4 </span><span class="sxs-lookup"><span data-stu-id="dd54c-122">4</span></span>|<span data-ttu-id="dd54c-123">Ошибка при анализе покрытия</span><span class="sxs-lookup"><span data-stu-id="dd54c-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="dd54c-124">нотаппликабле</span><span class="sxs-lookup"><span data-stu-id="dd54c-124">notApplicable</span></span>|<span data-ttu-id="dd54c-125">5 </span><span class="sxs-lookup"><span data-stu-id="dd54c-125">5</span></span>|<span data-ttu-id="dd54c-126">Нет параметров групповой политики в объекте групповой политики</span><span class="sxs-lookup"><span data-stu-id="dd54c-126">No Group Policy settings in GPO</span></span>|




