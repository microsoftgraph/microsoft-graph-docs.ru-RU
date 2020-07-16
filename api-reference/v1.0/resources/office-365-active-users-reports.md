---
title: Отчеты об активных пользователях Microsoft 365
description: С помощью отчетов Microsoft 365 активные пользователи могут узнать, сколько лицензий используются отдельными пользователями в вашей организации, и получить подробные сведения о том, какие пользователи используют продукты. Эти отчеты помогут администраторам определить редко используемые продукты или выявить пользователей, которым, возможно, необходимо дополнительное обучение или информация.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 041bbe180df2225383d704002d06359334fb8d84
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898165"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="5c752-104">Отчеты об активных пользователях Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5c752-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="5c752-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c752-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c752-106">С помощью отчетов Microsoft 365 активные пользователи могут узнать, сколько лицензий используются отдельными пользователями в вашей организации, и получить подробные сведения о том, какие пользователи используют продукты.</span><span class="sxs-lookup"><span data-stu-id="5c752-106">You can use the Microsoft 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="5c752-107">Эти отчеты помогут администраторам определить редко используемые продукты или выявить пользователей, которым, возможно, необходимо дополнительное обучение или информация.</span><span class="sxs-lookup"><span data-stu-id="5c752-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="5c752-108">**Примечание:** Подробные сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 отчеты об активных пользователях](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="5c752-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="5c752-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="5c752-109">Reports</span></span>
| <span data-ttu-id="5c752-110">Функция</span><span class="sxs-lookup"><span data-stu-id="5c752-110">Function</span></span>                                 | <span data-ttu-id="5c752-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c752-111">Return Type</span></span> | <span data-ttu-id="5c752-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5c752-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="5c752-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="5c752-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="5c752-114">Stream</span><span class="sxs-lookup"><span data-stu-id="5c752-114">Stream</span></span>      | <span data-ttu-id="5c752-115">Получение сведений о активных пользователях Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5c752-115">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="5c752-116">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="5c752-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="5c752-117">Stream</span><span class="sxs-lookup"><span data-stu-id="5c752-117">Stream</span></span>      | <span data-ttu-id="5c752-118">Узнайте, сколько активных пользователей в день было у каждого продукта в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5c752-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="5c752-119">Получение количества пользователей по службам</span><span class="sxs-lookup"><span data-stu-id="5c752-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="5c752-120">Поток</span><span class="sxs-lookup"><span data-stu-id="5c752-120">Stream</span></span>      | <span data-ttu-id="5c752-121">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="5c752-121">Get the count of users by activity type and service.</span></span> |
