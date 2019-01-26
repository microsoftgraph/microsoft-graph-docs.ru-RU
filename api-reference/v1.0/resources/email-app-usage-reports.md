---
title: Отчеты об использовании почтовых приложений
description: Эти отчеты позволяют узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 00adbec446cda1ea6855c7f52e847f88f42c65bd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574441"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="f4069-104">Отчеты об использовании почтовых приложений</span><span class="sxs-lookup"><span data-stu-id="f4069-104">Email app usage reports</span></span>

<span data-ttu-id="f4069-105">Эти отчеты позволяют узнать, сколько почтовых приложений используется для подключения к Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f4069-105">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="f4069-106">Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.</span><span class="sxs-lookup"><span data-stu-id="f4069-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="f4069-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="f4069-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="f4069-108">Отчеты</span><span class="sxs-lookup"><span data-stu-id="f4069-108">Reports</span></span>

| <span data-ttu-id="f4069-109">Функция</span><span class="sxs-lookup"><span data-stu-id="f4069-109">Function</span></span>                                 | <span data-ttu-id="f4069-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f4069-110">Return Type</span></span> | <span data-ttu-id="f4069-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f4069-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="f4069-112">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="f4069-112">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="f4069-113">Поток</span><span class="sxs-lookup"><span data-stu-id="f4069-113">Stream</span></span>      | <span data-ttu-id="f4069-114">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="f4069-114">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="f4069-115">Получение количества пользователей по приложениям</span><span class="sxs-lookup"><span data-stu-id="f4069-115">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="f4069-116">Поток</span><span class="sxs-lookup"><span data-stu-id="f4069-116">Stream</span></span>      | <span data-ttu-id="f4069-117">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="f4069-117">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="f4069-118">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="f4069-118">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="f4069-119">Поток</span><span class="sxs-lookup"><span data-stu-id="f4069-119">Stream</span></span>      | <span data-ttu-id="f4069-120">Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="f4069-120">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="f4069-121">Получение количества пользователей по версиям</span><span class="sxs-lookup"><span data-stu-id="f4069-121">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="f4069-122">Поток</span><span class="sxs-lookup"><span data-stu-id="f4069-122">Stream</span></span>      | <span data-ttu-id="f4069-123">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="f4069-123">Get the count of unique users by Outlook desktop version.</span></span> |
