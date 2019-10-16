---
title: тип перечисления Девицеманажементрепортстатус
description: Возможные состояния, связанные с созданным отчетом
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbc348dc8b95d03f6811815efda293e68a695ea2
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539038"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="b0b1c-103">тип перечисления Девицеманажементрепортстатус</span><span class="sxs-lookup"><span data-stu-id="b0b1c-103">deviceManagementReportStatus enum type</span></span>

> <span data-ttu-id="b0b1c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0b1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0b1c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0b1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0b1c-106">Возможные состояния, связанные с созданным отчетом</span><span class="sxs-lookup"><span data-stu-id="b0b1c-106">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="b0b1c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b0b1c-107">Members</span></span>
|<span data-ttu-id="b0b1c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b0b1c-108">Member</span></span>|<span data-ttu-id="b0b1c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b0b1c-109">Value</span></span>|<span data-ttu-id="b0b1c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b0b1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0b1c-111">unknown</span><span class="sxs-lookup"><span data-stu-id="b0b1c-111">unknown</span></span>|<span data-ttu-id="b0b1c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b0b1c-112">0</span></span>|<span data-ttu-id="b0b1c-113">Состояние создания отчета неизвестно</span><span class="sxs-lookup"><span data-stu-id="b0b1c-113">Report generation status is unknown</span></span>|
|<span data-ttu-id="b0b1c-114">notStarted</span><span class="sxs-lookup"><span data-stu-id="b0b1c-114">notStarted</span></span>|<span data-ttu-id="b0b1c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b0b1c-115">1</span></span>|<span data-ttu-id="b0b1c-116">Создание отчета не начато</span><span class="sxs-lookup"><span data-stu-id="b0b1c-116">Report generation has not started</span></span>|
|<span data-ttu-id="b0b1c-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="b0b1c-117">inProgress</span></span>|<span data-ttu-id="b0b1c-118">2</span><span class="sxs-lookup"><span data-stu-id="b0b1c-118">2</span></span>|<span data-ttu-id="b0b1c-119">Идет создание отчета</span><span class="sxs-lookup"><span data-stu-id="b0b1c-119">Report generation is in progress</span></span>|
|<span data-ttu-id="b0b1c-120">готовы</span><span class="sxs-lookup"><span data-stu-id="b0b1c-120">completed</span></span>|<span data-ttu-id="b0b1c-121">4</span><span class="sxs-lookup"><span data-stu-id="b0b1c-121">3</span></span>|<span data-ttu-id="b0b1c-122">Создание отчета завершено</span><span class="sxs-lookup"><span data-stu-id="b0b1c-122">Report generation is completed</span></span>|
|<span data-ttu-id="b0b1c-123">сбоев</span><span class="sxs-lookup"><span data-stu-id="b0b1c-123">failed</span></span>|<span data-ttu-id="b0b1c-124">4 </span><span class="sxs-lookup"><span data-stu-id="b0b1c-124">4</span></span>|<span data-ttu-id="b0b1c-125">Не удалось создать отчет</span><span class="sxs-lookup"><span data-stu-id="b0b1c-125">Report generation has failed</span></span>|



