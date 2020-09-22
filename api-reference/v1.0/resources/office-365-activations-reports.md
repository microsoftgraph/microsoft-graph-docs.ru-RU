---
title: Отчеты об активации Microsoft 365
description: Отчеты об активации Microsoft 365 могут предоставить представление о том, какие пользователи активировали подписки Microsoft 365 по крайней мере на одном устройстве. В этих отчетах представлены сведения об активации подписки на Microsoft 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ebca76ca3fe9356839636e7dca29293b083c13ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970672"
---
# <a name="microsoft-365-activations-reports"></a><span data-ttu-id="7ee94-105">Отчеты об активации Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7ee94-105">Microsoft 365 activations reports</span></span>

<span data-ttu-id="7ee94-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ee94-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ee94-107">Отчеты об активации Microsoft 365 могут предоставить представление о том, какие пользователи активировали подписки Microsoft 365 по крайней мере на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="7ee94-107">The Microsoft 365 activation reports can give you a view of which users have activated their Microsoft 365 subscriptions on at least one device.</span></span> <span data-ttu-id="7ee94-108">В этих отчетах представлены сведения об активации подписки на Microsoft 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах.</span><span class="sxs-lookup"><span data-stu-id="7ee94-108">These reports provide a breakdown of the Microsoft 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="7ee94-109">Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.</span><span class="sxs-lookup"><span data-stu-id="7ee94-109">These reports could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="7ee94-110">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports — активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="7ee94-110">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="7ee94-111">Отчеты</span><span class="sxs-lookup"><span data-stu-id="7ee94-111">Reports</span></span>
| <span data-ttu-id="7ee94-112">Функция</span><span class="sxs-lookup"><span data-stu-id="7ee94-112">Function</span></span>                                 | <span data-ttu-id="7ee94-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ee94-113">Return Type</span></span> | <span data-ttu-id="7ee94-114">Описание</span><span class="sxs-lookup"><span data-stu-id="7ee94-114">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="7ee94-115">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="7ee94-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="7ee94-116">Stream</span><span class="sxs-lookup"><span data-stu-id="7ee94-116">Stream</span></span>      | <span data-ttu-id="7ee94-117">Получение сведений о пользователях, которые активировали Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7ee94-117">Get details about users who have activated Microsoft 365.</span></span> |
| [<span data-ttu-id="7ee94-118">Получение количества активаций</span><span class="sxs-lookup"><span data-stu-id="7ee94-118">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="7ee94-119">Поток</span><span class="sxs-lookup"><span data-stu-id="7ee94-119">Stream</span></span>      | <span data-ttu-id="7ee94-120">Получение числа активаций Microsoft 365 на настольных компьютерах и устройствах.</span><span class="sxs-lookup"><span data-stu-id="7ee94-120">Get the count of Microsoft 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="7ee94-121">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="7ee94-121">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="7ee94-122">Stream</span><span class="sxs-lookup"><span data-stu-id="7ee94-122">Stream</span></span>      | <span data-ttu-id="7ee94-123">Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="7ee94-123">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |

