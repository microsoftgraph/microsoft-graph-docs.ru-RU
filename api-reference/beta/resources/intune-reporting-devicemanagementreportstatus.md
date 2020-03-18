---
title: тип перечисления Девицеманажементрепортстатус
description: Возможные состояния, связанные с созданным отчетом
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c5578c11ae322fd1745cb5ed5d2f74091997be65
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772309"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="21ec7-103">тип перечисления Девицеманажементрепортстатус</span><span class="sxs-lookup"><span data-stu-id="21ec7-103">deviceManagementReportStatus enum type</span></span>

> <span data-ttu-id="21ec7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21ec7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21ec7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21ec7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21ec7-106">Возможные состояния, связанные с созданным отчетом</span><span class="sxs-lookup"><span data-stu-id="21ec7-106">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="21ec7-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="21ec7-107">Members</span></span>
|<span data-ttu-id="21ec7-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="21ec7-108">Member</span></span>|<span data-ttu-id="21ec7-109">Значение</span><span class="sxs-lookup"><span data-stu-id="21ec7-109">Value</span></span>|<span data-ttu-id="21ec7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="21ec7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ec7-111">unknown</span><span class="sxs-lookup"><span data-stu-id="21ec7-111">unknown</span></span>|<span data-ttu-id="21ec7-112">нуль</span><span class="sxs-lookup"><span data-stu-id="21ec7-112">0</span></span>|<span data-ttu-id="21ec7-113">Состояние создания отчета неизвестно</span><span class="sxs-lookup"><span data-stu-id="21ec7-113">Report generation status is unknown</span></span>|
|<span data-ttu-id="21ec7-114">notStarted</span><span class="sxs-lookup"><span data-stu-id="21ec7-114">notStarted</span></span>|<span data-ttu-id="21ec7-115">1,1</span><span class="sxs-lookup"><span data-stu-id="21ec7-115">1</span></span>|<span data-ttu-id="21ec7-116">Создание отчета не начато</span><span class="sxs-lookup"><span data-stu-id="21ec7-116">Report generation has not started</span></span>|
|<span data-ttu-id="21ec7-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="21ec7-117">inProgress</span></span>|<span data-ttu-id="21ec7-118">2</span><span class="sxs-lookup"><span data-stu-id="21ec7-118">2</span></span>|<span data-ttu-id="21ec7-119">Идет создание отчета</span><span class="sxs-lookup"><span data-stu-id="21ec7-119">Report generation is in progress</span></span>|
|<span data-ttu-id="21ec7-120">готовы</span><span class="sxs-lookup"><span data-stu-id="21ec7-120">completed</span></span>|<span data-ttu-id="21ec7-121">4</span><span class="sxs-lookup"><span data-stu-id="21ec7-121">3</span></span>|<span data-ttu-id="21ec7-122">Создание отчета завершено</span><span class="sxs-lookup"><span data-stu-id="21ec7-122">Report generation is completed</span></span>|
|<span data-ttu-id="21ec7-123">сбоев</span><span class="sxs-lookup"><span data-stu-id="21ec7-123">failed</span></span>|<span data-ttu-id="21ec7-124">4 </span><span class="sxs-lookup"><span data-stu-id="21ec7-124">4</span></span>|<span data-ttu-id="21ec7-125">Не удалось создать отчет</span><span class="sxs-lookup"><span data-stu-id="21ec7-125">Report generation has failed</span></span>|



