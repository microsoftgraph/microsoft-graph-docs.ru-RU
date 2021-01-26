---
title: Отчеты об активациях Microsoft 365
description: Отчеты об активации Microsoft 365 могут дать вам представление о том, какие пользователи активировали подписки Microsoft 365 хотя бы на одном устройстве. Эти отчеты предоставляют разбивку по активациям подписок Microsoft 365 профессиональныйplus, Project и Visio Pro для Office 365, а также разбивку активаций на настольных компьютерах и устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 30d9fa1799367e0589115c56dd069db6ca7b1ff9
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981048"
---
# <a name="microsoft-365-activations-reports"></a><span data-ttu-id="5d2a8-105">Отчеты об активациях Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5d2a8-105">Microsoft 365 activations reports</span></span>

<span data-ttu-id="5d2a8-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d2a8-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d2a8-107">Отчеты об активации Microsoft 365 могут дать вам представление о том, какие пользователи активировали подписки Microsoft 365 хотя бы на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="5d2a8-107">The Microsoft 365 activation reports can give you a view of which users have activated their Microsoft 365 subscriptions on at least one device.</span></span> <span data-ttu-id="5d2a8-108">Эти отчеты предоставляют разбивку по активациям подписок Microsoft 365 профессиональныйplus, Project и Visio Pro для Office 365, а также разбивку активаций на настольных компьютерах и устройствах.</span><span class="sxs-lookup"><span data-stu-id="5d2a8-108">These reports provide a breakdown of the Microsoft 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="5d2a8-109">Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.</span><span class="sxs-lookup"><span data-stu-id="5d2a8-109">These reports could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="5d2a8-110">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в отчетах [Microsoft 365 Microsoft Office активации.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)</span><span class="sxs-lookup"><span data-stu-id="5d2a8-110">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="5d2a8-111">Отчеты</span><span class="sxs-lookup"><span data-stu-id="5d2a8-111">Reports</span></span>
| <span data-ttu-id="5d2a8-112">Функция</span><span class="sxs-lookup"><span data-stu-id="5d2a8-112">Function</span></span>                                 | <span data-ttu-id="5d2a8-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d2a8-113">Return Type</span></span> | <span data-ttu-id="5d2a8-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5d2a8-114">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="5d2a8-115">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="5d2a8-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="5d2a8-116">Stream</span><span class="sxs-lookup"><span data-stu-id="5d2a8-116">Stream</span></span>      | <span data-ttu-id="5d2a8-117">Получите сведения о пользователях, активировавших Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5d2a8-117">Get details about users who have activated Microsoft 365.</span></span> |
| [<span data-ttu-id="5d2a8-118">Получение количества активаций</span><span class="sxs-lookup"><span data-stu-id="5d2a8-118">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="5d2a8-119">Поток</span><span class="sxs-lookup"><span data-stu-id="5d2a8-119">Stream</span></span>      | <span data-ttu-id="5d2a8-120">Получите количество активаций Microsoft 365 на настольных компьютерах и устройствах.</span><span class="sxs-lookup"><span data-stu-id="5d2a8-120">Get the count of Microsoft 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="5d2a8-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="5d2a8-121">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="5d2a8-122">Stream</span><span class="sxs-lookup"><span data-stu-id="5d2a8-122">Stream</span></span>      | <span data-ttu-id="5d2a8-123">Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="5d2a8-123">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |

