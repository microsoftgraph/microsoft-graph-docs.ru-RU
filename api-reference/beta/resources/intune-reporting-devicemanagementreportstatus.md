---
title: тип перечисления Девицеманажементрепортстатус
description: Возможные состояния, связанные с созданным отчетом
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eb85ade317129c1bae790dff43b42d5c839d45d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287678"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="053d9-103">тип перечисления Девицеманажементрепортстатус</span><span class="sxs-lookup"><span data-stu-id="053d9-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="053d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="053d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="053d9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="053d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="053d9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="053d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="053d9-107">Возможные состояния, связанные с созданным отчетом</span><span class="sxs-lookup"><span data-stu-id="053d9-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="053d9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="053d9-108">Members</span></span>
|<span data-ttu-id="053d9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="053d9-109">Member</span></span>|<span data-ttu-id="053d9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="053d9-110">Value</span></span>|<span data-ttu-id="053d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="053d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="053d9-112">unknown</span><span class="sxs-lookup"><span data-stu-id="053d9-112">unknown</span></span>|<span data-ttu-id="053d9-113">нуль</span><span class="sxs-lookup"><span data-stu-id="053d9-113">0</span></span>|<span data-ttu-id="053d9-114">Состояние создания отчета неизвестно</span><span class="sxs-lookup"><span data-stu-id="053d9-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="053d9-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="053d9-115">notStarted</span></span>|<span data-ttu-id="053d9-116">1,1</span><span class="sxs-lookup"><span data-stu-id="053d9-116">1</span></span>|<span data-ttu-id="053d9-117">Создание отчета не начато</span><span class="sxs-lookup"><span data-stu-id="053d9-117">Report generation has not started</span></span>|
|<span data-ttu-id="053d9-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="053d9-118">inProgress</span></span>|<span data-ttu-id="053d9-119">2</span><span class="sxs-lookup"><span data-stu-id="053d9-119">2</span></span>|<span data-ttu-id="053d9-120">Идет создание отчета</span><span class="sxs-lookup"><span data-stu-id="053d9-120">Report generation is in progress</span></span>|
|<span data-ttu-id="053d9-121">готовы</span><span class="sxs-lookup"><span data-stu-id="053d9-121">completed</span></span>|<span data-ttu-id="053d9-122">4</span><span class="sxs-lookup"><span data-stu-id="053d9-122">3</span></span>|<span data-ttu-id="053d9-123">Создание отчета завершено</span><span class="sxs-lookup"><span data-stu-id="053d9-123">Report generation is completed</span></span>|
|<span data-ttu-id="053d9-124">сбоев</span><span class="sxs-lookup"><span data-stu-id="053d9-124">failed</span></span>|<span data-ttu-id="053d9-125">4 </span><span class="sxs-lookup"><span data-stu-id="053d9-125">4</span></span>|<span data-ttu-id="053d9-126">Не удалось создать отчет</span><span class="sxs-lookup"><span data-stu-id="053d9-126">Report generation has failed</span></span>|




