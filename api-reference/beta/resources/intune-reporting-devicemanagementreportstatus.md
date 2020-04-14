---
title: тип перечисления Девицеманажементрепортстатус
description: Возможные состояния, связанные с созданным отчетом
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9f7ab2225d862dc14d1687e286cc71681988f0f8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453196"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="383da-103">тип перечисления Девицеманажементрепортстатус</span><span class="sxs-lookup"><span data-stu-id="383da-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="383da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="383da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="383da-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="383da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="383da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="383da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="383da-107">Возможные состояния, связанные с созданным отчетом</span><span class="sxs-lookup"><span data-stu-id="383da-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="383da-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="383da-108">Members</span></span>
|<span data-ttu-id="383da-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="383da-109">Member</span></span>|<span data-ttu-id="383da-110">Значение</span><span class="sxs-lookup"><span data-stu-id="383da-110">Value</span></span>|<span data-ttu-id="383da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="383da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="383da-112">unknown</span><span class="sxs-lookup"><span data-stu-id="383da-112">unknown</span></span>|<span data-ttu-id="383da-113">нуль</span><span class="sxs-lookup"><span data-stu-id="383da-113">0</span></span>|<span data-ttu-id="383da-114">Состояние создания отчета неизвестно</span><span class="sxs-lookup"><span data-stu-id="383da-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="383da-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="383da-115">notStarted</span></span>|<span data-ttu-id="383da-116">1,1</span><span class="sxs-lookup"><span data-stu-id="383da-116">1</span></span>|<span data-ttu-id="383da-117">Создание отчета не начато</span><span class="sxs-lookup"><span data-stu-id="383da-117">Report generation has not started</span></span>|
|<span data-ttu-id="383da-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="383da-118">inProgress</span></span>|<span data-ttu-id="383da-119">2</span><span class="sxs-lookup"><span data-stu-id="383da-119">2</span></span>|<span data-ttu-id="383da-120">Идет создание отчета</span><span class="sxs-lookup"><span data-stu-id="383da-120">Report generation is in progress</span></span>|
|<span data-ttu-id="383da-121">готовы</span><span class="sxs-lookup"><span data-stu-id="383da-121">completed</span></span>|<span data-ttu-id="383da-122">4</span><span class="sxs-lookup"><span data-stu-id="383da-122">3</span></span>|<span data-ttu-id="383da-123">Создание отчета завершено</span><span class="sxs-lookup"><span data-stu-id="383da-123">Report generation is completed</span></span>|
|<span data-ttu-id="383da-124">сбоев</span><span class="sxs-lookup"><span data-stu-id="383da-124">failed</span></span>|<span data-ttu-id="383da-125">4 </span><span class="sxs-lookup"><span data-stu-id="383da-125">4</span></span>|<span data-ttu-id="383da-126">Не удалось создать отчет</span><span class="sxs-lookup"><span data-stu-id="383da-126">Report generation has failed</span></span>|



