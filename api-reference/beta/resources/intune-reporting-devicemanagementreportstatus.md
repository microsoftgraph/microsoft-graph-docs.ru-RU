---
title: тип перечисления Девицеманажементрепортстатус
description: Возможные состояния, связанные с созданным отчетом
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e549e2ca96e272930c13aa07f0e35e2143e96c2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527513"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="66caf-103">тип перечисления Девицеманажементрепортстатус</span><span class="sxs-lookup"><span data-stu-id="66caf-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="66caf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="66caf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66caf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66caf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66caf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66caf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66caf-107">Возможные состояния, связанные с созданным отчетом</span><span class="sxs-lookup"><span data-stu-id="66caf-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="66caf-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="66caf-108">Members</span></span>
|<span data-ttu-id="66caf-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="66caf-109">Member</span></span>|<span data-ttu-id="66caf-110">Значение</span><span class="sxs-lookup"><span data-stu-id="66caf-110">Value</span></span>|<span data-ttu-id="66caf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66caf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66caf-112">unknown</span><span class="sxs-lookup"><span data-stu-id="66caf-112">unknown</span></span>|<span data-ttu-id="66caf-113">нуль</span><span class="sxs-lookup"><span data-stu-id="66caf-113">0</span></span>|<span data-ttu-id="66caf-114">Состояние создания отчета неизвестно</span><span class="sxs-lookup"><span data-stu-id="66caf-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="66caf-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="66caf-115">notStarted</span></span>|<span data-ttu-id="66caf-116">1 </span><span class="sxs-lookup"><span data-stu-id="66caf-116">1</span></span>|<span data-ttu-id="66caf-117">Создание отчета не начато</span><span class="sxs-lookup"><span data-stu-id="66caf-117">Report generation has not started</span></span>|
|<span data-ttu-id="66caf-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="66caf-118">inProgress</span></span>|<span data-ttu-id="66caf-119">2 </span><span class="sxs-lookup"><span data-stu-id="66caf-119">2</span></span>|<span data-ttu-id="66caf-120">Идет создание отчета</span><span class="sxs-lookup"><span data-stu-id="66caf-120">Report generation is in progress</span></span>|
|<span data-ttu-id="66caf-121">готовы</span><span class="sxs-lookup"><span data-stu-id="66caf-121">completed</span></span>|<span data-ttu-id="66caf-122">3 </span><span class="sxs-lookup"><span data-stu-id="66caf-122">3</span></span>|<span data-ttu-id="66caf-123">Создание отчета завершено</span><span class="sxs-lookup"><span data-stu-id="66caf-123">Report generation is completed</span></span>|
|<span data-ttu-id="66caf-124">сбоев</span><span class="sxs-lookup"><span data-stu-id="66caf-124">failed</span></span>|<span data-ttu-id="66caf-125">4 </span><span class="sxs-lookup"><span data-stu-id="66caf-125">4</span></span>|<span data-ttu-id="66caf-126">Не удалось создать отчет</span><span class="sxs-lookup"><span data-stu-id="66caf-126">Report generation has failed</span></span>|



