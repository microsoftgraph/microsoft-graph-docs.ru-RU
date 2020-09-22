---
title: Отчеты об активных пользователях Microsoft 365
description: Вы можете использовать отчет по активным пользователям Microsoft 365, чтобы узнать, сколько лицензий используется отдельными пользователями в вашей организации, и детализировать информацию о том, какие пользователи используют продукты. Этот отчет поможет администраторам выяснить, какие продукты используются редко, или определить пользователей, которым могут понадобиться дополнительное обучение и сведения.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 3d795c3308b7c1494bbff2a24545ba4ca8053583
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021254"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="5cdfb-104">Отчеты об активных пользователях Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5cdfb-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="5cdfb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cdfb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cdfb-106">Вы можете использовать отчет по активным пользователям Microsoft 365, чтобы узнать, сколько лицензий используется отдельными пользователями в вашей организации, и детализировать информацию о том, какие пользователи используют продукты.</span><span class="sxs-lookup"><span data-stu-id="5cdfb-106">You can use the Microsoft 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="5cdfb-107">Этот отчет поможет администраторам выяснить, какие продукты используются редко, или определить пользователей, которым могут понадобиться дополнительное обучение и сведения.</span><span class="sxs-lookup"><span data-stu-id="5cdfb-107">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="5cdfb-108">**Примечание:** Подробные сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 отчеты об активных пользователях](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="5cdfb-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="5cdfb-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="5cdfb-109">Reports</span></span>
| <span data-ttu-id="5cdfb-110">Функция</span><span class="sxs-lookup"><span data-stu-id="5cdfb-110">Function</span></span>                                 | <span data-ttu-id="5cdfb-111">Возвращаемый тип CSV</span><span class="sxs-lookup"><span data-stu-id="5cdfb-111">CSV return type</span></span> | <span data-ttu-id="5cdfb-112">Возвращаемый тип JSON</span><span class="sxs-lookup"><span data-stu-id="5cdfb-112">JSON return type</span></span>                         | <span data-ttu-id="5cdfb-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5cdfb-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5cdfb-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="5cdfb-114">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="5cdfb-115">Stream</span><span class="sxs-lookup"><span data-stu-id="5cdfb-115">Stream</span></span>          | [<span data-ttu-id="5cdfb-116">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="5cdfb-116">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="5cdfb-117">Получение сведений о активных пользователях Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5cdfb-117">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="5cdfb-118">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="5cdfb-118">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="5cdfb-119">Stream</span><span class="sxs-lookup"><span data-stu-id="5cdfb-119">Stream</span></span>          | [<span data-ttu-id="5cdfb-120">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="5cdfb-120">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="5cdfb-121">Узнайте, сколько активных пользователей в день было у каждого продукта в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5cdfb-121">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="5cdfb-122">Получение количества пользователей по службам</span><span class="sxs-lookup"><span data-stu-id="5cdfb-122">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="5cdfb-123">Поток</span><span class="sxs-lookup"><span data-stu-id="5cdfb-123">Stream</span></span>          | [<span data-ttu-id="5cdfb-124">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="5cdfb-124">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="5cdfb-125">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="5cdfb-125">Get the count of users by activity type and service.</span></span> |


