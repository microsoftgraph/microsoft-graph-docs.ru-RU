---
title: тип перечисления Девицеманажементрепортстатус
description: Возможные состояния, связанные с созданным отчетом
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a73f9b552dd98bcb141e607666cb9570f88bc9ec
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735143"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="27405-103">тип перечисления Девицеманажементрепортстатус</span><span class="sxs-lookup"><span data-stu-id="27405-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="27405-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27405-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27405-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27405-107">Возможные состояния, связанные с созданным отчетом</span><span class="sxs-lookup"><span data-stu-id="27405-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="27405-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="27405-108">Members</span></span>
|<span data-ttu-id="27405-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="27405-109">Member</span></span>|<span data-ttu-id="27405-110">Значение</span><span class="sxs-lookup"><span data-stu-id="27405-110">Value</span></span>|<span data-ttu-id="27405-111">Описание</span><span class="sxs-lookup"><span data-stu-id="27405-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27405-112">unknown</span><span class="sxs-lookup"><span data-stu-id="27405-112">unknown</span></span>|<span data-ttu-id="27405-113">нуль</span><span class="sxs-lookup"><span data-stu-id="27405-113">0</span></span>|<span data-ttu-id="27405-114">Состояние создания отчета неизвестно</span><span class="sxs-lookup"><span data-stu-id="27405-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="27405-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="27405-115">notStarted</span></span>|<span data-ttu-id="27405-116">1,1</span><span class="sxs-lookup"><span data-stu-id="27405-116">1</span></span>|<span data-ttu-id="27405-117">Создание отчета не начато</span><span class="sxs-lookup"><span data-stu-id="27405-117">Report generation has not started</span></span>|
|<span data-ttu-id="27405-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="27405-118">inProgress</span></span>|<span data-ttu-id="27405-119">2</span><span class="sxs-lookup"><span data-stu-id="27405-119">2</span></span>|<span data-ttu-id="27405-120">Идет создание отчета</span><span class="sxs-lookup"><span data-stu-id="27405-120">Report generation is in progress</span></span>|
|<span data-ttu-id="27405-121">готовы</span><span class="sxs-lookup"><span data-stu-id="27405-121">completed</span></span>|<span data-ttu-id="27405-122">4</span><span class="sxs-lookup"><span data-stu-id="27405-122">3</span></span>|<span data-ttu-id="27405-123">Создание отчета завершено</span><span class="sxs-lookup"><span data-stu-id="27405-123">Report generation is completed</span></span>|
|<span data-ttu-id="27405-124">сбоев</span><span class="sxs-lookup"><span data-stu-id="27405-124">failed</span></span>|<span data-ttu-id="27405-125">4 </span><span class="sxs-lookup"><span data-stu-id="27405-125">4</span></span>|<span data-ttu-id="27405-126">Не удалось создать отчет</span><span class="sxs-lookup"><span data-stu-id="27405-126">Report generation has failed</span></span>|





