---
title: Отчеты об активных пользователях Office 365
description: Эти отчеты позволяют узнать, сколько лицензий используется в вашей организации, и выяснить, кто какие продукты использует. Эти отчеты помогут администраторам определить редко используемые продукты или выявить пользователей, которым, возможно, необходимо дополнительное обучение или информация.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 163eab83bfcb5089ec21d449d90840384c12e4ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447348"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="78fce-104">Отчеты об активных пользователях Office 365</span><span class="sxs-lookup"><span data-stu-id="78fce-104">Office 365 active users reports</span></span>

<span data-ttu-id="78fce-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="78fce-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78fce-106">Эти отчеты позволяют узнать, сколько лицензий используется в вашей организации, и выяснить, кто какие продукты использует.</span><span class="sxs-lookup"><span data-stu-id="78fce-106">You can use the Office 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="78fce-107">Эти отчеты помогут администраторам определить редко используемые продукты или выявить пользователей, которым, возможно, необходимо дополнительное обучение или информация.</span><span class="sxs-lookup"><span data-stu-id="78fce-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="78fce-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="78fce-108">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="78fce-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="78fce-109">Reports</span></span>
| <span data-ttu-id="78fce-110">Функция</span><span class="sxs-lookup"><span data-stu-id="78fce-110">Function</span></span>                                 | <span data-ttu-id="78fce-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78fce-111">Return Type</span></span> | <span data-ttu-id="78fce-112">Описание</span><span class="sxs-lookup"><span data-stu-id="78fce-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="78fce-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="78fce-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="78fce-114">Stream</span><span class="sxs-lookup"><span data-stu-id="78fce-114">Stream</span></span>      | <span data-ttu-id="78fce-115">Получите сведения об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="78fce-115">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="78fce-116">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="78fce-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="78fce-117">Stream</span><span class="sxs-lookup"><span data-stu-id="78fce-117">Stream</span></span>      | <span data-ttu-id="78fce-118">Узнайте, сколько активных пользователей в день было у каждого продукта в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="78fce-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="78fce-119">Получение количества пользователей по службам</span><span class="sxs-lookup"><span data-stu-id="78fce-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="78fce-120">Поток</span><span class="sxs-lookup"><span data-stu-id="78fce-120">Stream</span></span>      | <span data-ttu-id="78fce-121">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="78fce-121">Get the count of users by activity type and service.</span></span> |
