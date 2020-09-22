---
title: тип перечисления Девицеманажементрепортстатус
description: Возможные состояния, связанные с созданным отчетом
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fe2895f73857bb73262aaa9e90894da7e8028d22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079783"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="1bbf1-103">тип перечисления Девицеманажементрепортстатус</span><span class="sxs-lookup"><span data-stu-id="1bbf1-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="1bbf1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bbf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bbf1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bbf1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bbf1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bbf1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bbf1-107">Возможные состояния, связанные с созданным отчетом</span><span class="sxs-lookup"><span data-stu-id="1bbf1-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="1bbf1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1bbf1-108">Members</span></span>
|<span data-ttu-id="1bbf1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1bbf1-109">Member</span></span>|<span data-ttu-id="1bbf1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1bbf1-110">Value</span></span>|<span data-ttu-id="1bbf1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1bbf1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bbf1-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1bbf1-112">unknown</span></span>|<span data-ttu-id="1bbf1-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1bbf1-113">0</span></span>|<span data-ttu-id="1bbf1-114">Состояние создания отчета неизвестно</span><span class="sxs-lookup"><span data-stu-id="1bbf1-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="1bbf1-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="1bbf1-115">notStarted</span></span>|<span data-ttu-id="1bbf1-116">1 </span><span class="sxs-lookup"><span data-stu-id="1bbf1-116">1</span></span>|<span data-ttu-id="1bbf1-117">Создание отчета не начато</span><span class="sxs-lookup"><span data-stu-id="1bbf1-117">Report generation has not started</span></span>|
|<span data-ttu-id="1bbf1-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="1bbf1-118">inProgress</span></span>|<span data-ttu-id="1bbf1-119">2 </span><span class="sxs-lookup"><span data-stu-id="1bbf1-119">2</span></span>|<span data-ttu-id="1bbf1-120">Идет создание отчета</span><span class="sxs-lookup"><span data-stu-id="1bbf1-120">Report generation is in progress</span></span>|
|<span data-ttu-id="1bbf1-121">готовы</span><span class="sxs-lookup"><span data-stu-id="1bbf1-121">completed</span></span>|<span data-ttu-id="1bbf1-122">4</span><span class="sxs-lookup"><span data-stu-id="1bbf1-122">3</span></span>|<span data-ttu-id="1bbf1-123">Создание отчета завершено</span><span class="sxs-lookup"><span data-stu-id="1bbf1-123">Report generation is completed</span></span>|
|<span data-ttu-id="1bbf1-124">сбоев</span><span class="sxs-lookup"><span data-stu-id="1bbf1-124">failed</span></span>|<span data-ttu-id="1bbf1-125">4 </span><span class="sxs-lookup"><span data-stu-id="1bbf1-125">4</span></span>|<span data-ttu-id="1bbf1-126">Не удалось создать отчет</span><span class="sxs-lookup"><span data-stu-id="1bbf1-126">Report generation has failed</span></span>|






