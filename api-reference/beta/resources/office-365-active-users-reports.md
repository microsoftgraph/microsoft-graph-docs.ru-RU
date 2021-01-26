---
title: Отчеты об активных пользователях Microsoft 365
description: Вы можете использовать отчет об активных пользователях Microsoft 365, чтобы узнать, сколько лицензий на продукты используются пользователями в вашей организации, и получить более подробную информацию о том, какие пользователи используют какие продукты. Этот отчет поможет администраторам выяснить, какие продукты используются редко, или определить пользователей, которым могут понадобиться дополнительное обучение и сведения.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: ee227bf0413944bdd648de64f32bf4f6ab9f3d70
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980775"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="ac890-104">Отчеты об активных пользователях Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ac890-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="ac890-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac890-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac890-106">Вы можете использовать отчет об активных пользователях Microsoft 365, чтобы узнать, сколько лицензий на продукты используются пользователями в вашей организации, и получить более подробную информацию о том, какие пользователи используют какие продукты.</span><span class="sxs-lookup"><span data-stu-id="ac890-106">You can use the Microsoft 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="ac890-107">Этот отчет поможет администраторам выяснить, какие продукты используются редко, или определить пользователей, которым могут понадобиться дополнительное обучение и сведения.</span><span class="sxs-lookup"><span data-stu-id="ac890-107">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="ac890-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Активные Пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="ac890-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="ac890-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="ac890-109">Reports</span></span>
| <span data-ttu-id="ac890-110">Функция</span><span class="sxs-lookup"><span data-stu-id="ac890-110">Function</span></span>                                 | <span data-ttu-id="ac890-111">Тип возврата CSV</span><span class="sxs-lookup"><span data-stu-id="ac890-111">CSV return type</span></span> | <span data-ttu-id="ac890-112">Тип возврата JSON</span><span class="sxs-lookup"><span data-stu-id="ac890-112">JSON return type</span></span>                         | <span data-ttu-id="ac890-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ac890-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ac890-114">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="ac890-114">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="ac890-115">Stream</span><span class="sxs-lookup"><span data-stu-id="ac890-115">Stream</span></span>          | [<span data-ttu-id="ac890-116">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="ac890-116">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="ac890-117">Получение сведений об активных пользователях Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ac890-117">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="ac890-118">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="ac890-118">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="ac890-119">Stream</span><span class="sxs-lookup"><span data-stu-id="ac890-119">Stream</span></span>          | [<span data-ttu-id="ac890-120">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="ac890-120">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="ac890-121">Узнайте, сколько активных пользователей в день было у каждого продукта в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ac890-121">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="ac890-122">Получение количества пользователей по службам</span><span class="sxs-lookup"><span data-stu-id="ac890-122">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="ac890-123">Поток</span><span class="sxs-lookup"><span data-stu-id="ac890-123">Stream</span></span>          | [<span data-ttu-id="ac890-124">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="ac890-124">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="ac890-125">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="ac890-125">Get the count of users by activity type and service.</span></span> |


