---
title: Отчеты об активных пользователях Microsoft 365
description: Вы можете использовать отчеты об активных пользователях Microsoft 365, чтобы узнать, сколько лицензий на продукты используются пользователями в вашей организации, и получить более подробную информацию о том, какие пользователи используют какие продукты. Эти отчеты помогут администраторам определить редко используемые продукты или выявить пользователей, которым, возможно, необходимо дополнительное обучение или информация.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e795b58eaae7ecd428f1473b277cd6bc65cbf09d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981027"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="111f9-104">Отчеты об активных пользователях Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="111f9-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="111f9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="111f9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="111f9-106">Вы можете использовать отчеты об активных пользователях Microsoft 365, чтобы узнать, сколько лицензий на продукты используются пользователями в вашей организации, и получить более подробную информацию о том, какие пользователи используют какие продукты.</span><span class="sxs-lookup"><span data-stu-id="111f9-106">You can use the Microsoft 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="111f9-107">Эти отчеты помогут администраторам определить редко используемые продукты или выявить пользователей, которым, возможно, необходимо дополнительное обучение или информация.</span><span class="sxs-lookup"><span data-stu-id="111f9-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="111f9-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Активные Пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="111f9-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="111f9-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="111f9-109">Reports</span></span>
| <span data-ttu-id="111f9-110">Функция</span><span class="sxs-lookup"><span data-stu-id="111f9-110">Function</span></span>                                 | <span data-ttu-id="111f9-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="111f9-111">Return Type</span></span> | <span data-ttu-id="111f9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="111f9-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="111f9-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="111f9-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="111f9-114">Stream</span><span class="sxs-lookup"><span data-stu-id="111f9-114">Stream</span></span>      | <span data-ttu-id="111f9-115">Получение сведений об активных пользователях Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="111f9-115">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="111f9-116">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="111f9-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="111f9-117">Stream</span><span class="sxs-lookup"><span data-stu-id="111f9-117">Stream</span></span>      | <span data-ttu-id="111f9-118">Узнайте, сколько активных пользователей в день было у каждого продукта в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="111f9-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="111f9-119">Получение количества пользователей по службам</span><span class="sxs-lookup"><span data-stu-id="111f9-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="111f9-120">Поток</span><span class="sxs-lookup"><span data-stu-id="111f9-120">Stream</span></span>      | <span data-ttu-id="111f9-121">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="111f9-121">Get the count of users by activity type and service.</span></span> |

