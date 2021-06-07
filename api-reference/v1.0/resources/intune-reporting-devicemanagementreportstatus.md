---
title: тип enum deviceManagementReportStatus
description: Возможные состояния, связанные с созданным отчетом
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b448d95d4aa25717e313d92f8b2a4e035228cf1a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752077"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="89960-103">тип enum deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="89960-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="89960-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89960-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89960-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89960-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89960-106">Возможные состояния, связанные с созданным отчетом</span><span class="sxs-lookup"><span data-stu-id="89960-106">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="89960-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="89960-107">Members</span></span>
|<span data-ttu-id="89960-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="89960-108">Member</span></span>|<span data-ttu-id="89960-109">Значение</span><span class="sxs-lookup"><span data-stu-id="89960-109">Value</span></span>|<span data-ttu-id="89960-110">Описание</span><span class="sxs-lookup"><span data-stu-id="89960-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89960-111">unknown</span><span class="sxs-lookup"><span data-stu-id="89960-111">unknown</span></span>|<span data-ttu-id="89960-112">0</span><span class="sxs-lookup"><span data-stu-id="89960-112">0</span></span>|<span data-ttu-id="89960-113">Состояние генерации отчетов неизвестно</span><span class="sxs-lookup"><span data-stu-id="89960-113">Report generation status is unknown</span></span>|
|<span data-ttu-id="89960-114">notStarted</span><span class="sxs-lookup"><span data-stu-id="89960-114">notStarted</span></span>|<span data-ttu-id="89960-115">1</span><span class="sxs-lookup"><span data-stu-id="89960-115">1</span></span>|<span data-ttu-id="89960-116">Генерация отчетов не началась</span><span class="sxs-lookup"><span data-stu-id="89960-116">Report generation has not started</span></span>|
|<span data-ttu-id="89960-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="89960-117">inProgress</span></span>|<span data-ttu-id="89960-118">2</span><span class="sxs-lookup"><span data-stu-id="89960-118">2</span></span>|<span data-ttu-id="89960-119">Продолжается генерация отчетов</span><span class="sxs-lookup"><span data-stu-id="89960-119">Report generation is in progress</span></span>|
|<span data-ttu-id="89960-120">завершено</span><span class="sxs-lookup"><span data-stu-id="89960-120">completed</span></span>|<span data-ttu-id="89960-121">3</span><span class="sxs-lookup"><span data-stu-id="89960-121">3</span></span>|<span data-ttu-id="89960-122">Завершено поколение отчетов</span><span class="sxs-lookup"><span data-stu-id="89960-122">Report generation is completed</span></span>|
|<span data-ttu-id="89960-123">не удалось</span><span class="sxs-lookup"><span data-stu-id="89960-123">failed</span></span>|<span data-ttu-id="89960-124">4 </span><span class="sxs-lookup"><span data-stu-id="89960-124">4</span></span>|<span data-ttu-id="89960-125">Сбой генерации отчетов</span><span class="sxs-lookup"><span data-stu-id="89960-125">Report generation has failed</span></span>|




