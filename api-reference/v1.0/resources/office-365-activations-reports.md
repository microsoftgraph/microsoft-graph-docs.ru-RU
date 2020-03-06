---
title: Отчеты об активации Office 365
description: Эти отчеты позволяют узнать, кто из пользователей активировал подписку на Office 365 по крайней мере на одном устройстве. Они содержат разбивку по активациям подписок на Office 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разбивку по активациям на компьютерах и мобильных устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: d01f3116f6a6a12753384ec41c2cee609b9b7f8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534182"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="ca27b-105">Отчеты об активации Office 365</span><span class="sxs-lookup"><span data-stu-id="ca27b-105">Office 365 activations reports</span></span>

<span data-ttu-id="ca27b-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca27b-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca27b-107">Эти отчеты позволяют узнать, кто из пользователей активировал подписку на Office 365 по крайней мере на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="ca27b-107">The Office 365 activation reports can give you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="ca27b-108">Они содержат разбивку по активациям подписок на Office 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разбивку по активациям на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="ca27b-108">These reports provide a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="ca27b-109">Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.</span><span class="sxs-lookup"><span data-stu-id="ca27b-109">These reports could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="ca27b-110">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="ca27b-110">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="ca27b-111">Отчеты</span><span class="sxs-lookup"><span data-stu-id="ca27b-111">Reports</span></span>
| <span data-ttu-id="ca27b-112">Функция</span><span class="sxs-lookup"><span data-stu-id="ca27b-112">Function</span></span>                                 | <span data-ttu-id="ca27b-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ca27b-113">Return Type</span></span> | <span data-ttu-id="ca27b-114">Описание</span><span class="sxs-lookup"><span data-stu-id="ca27b-114">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="ca27b-115">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="ca27b-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="ca27b-116">Stream</span><span class="sxs-lookup"><span data-stu-id="ca27b-116">Stream</span></span>      | <span data-ttu-id="ca27b-117">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="ca27b-117">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="ca27b-118">Получение количества активаций</span><span class="sxs-lookup"><span data-stu-id="ca27b-118">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="ca27b-119">Поток</span><span class="sxs-lookup"><span data-stu-id="ca27b-119">Stream</span></span>      | <span data-ttu-id="ca27b-120">Получите сведения о количестве активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="ca27b-120">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="ca27b-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="ca27b-121">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="ca27b-122">Stream</span><span class="sxs-lookup"><span data-stu-id="ca27b-122">Stream</span></span>      | <span data-ttu-id="ca27b-123">Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="ca27b-123">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
