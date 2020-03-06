---
title: Отчеты об использовании почтовых приложений
description: Эти отчеты позволяют узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 9ea3418dd065758fb2d623c9995b78126ea3d475
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532988"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="d27b1-104">Отчеты об использовании почтовых приложений</span><span class="sxs-lookup"><span data-stu-id="d27b1-104">Email app usage reports</span></span>

<span data-ttu-id="d27b1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d27b1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d27b1-106">Эти отчеты позволяют узнать, сколько почтовых приложений используется для подключения к Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="d27b1-106">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="d27b1-107">Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.</span><span class="sxs-lookup"><span data-stu-id="d27b1-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="d27b1-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="d27b1-108">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="d27b1-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="d27b1-109">Reports</span></span>

| <span data-ttu-id="d27b1-110">Функция</span><span class="sxs-lookup"><span data-stu-id="d27b1-110">Function</span></span>                                 | <span data-ttu-id="d27b1-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d27b1-111">Return Type</span></span> | <span data-ttu-id="d27b1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d27b1-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="d27b1-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="d27b1-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="d27b1-114">Stream</span><span class="sxs-lookup"><span data-stu-id="d27b1-114">Stream</span></span>      | <span data-ttu-id="d27b1-115">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="d27b1-115">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="d27b1-116">Получение количества пользователей по приложениям</span><span class="sxs-lookup"><span data-stu-id="d27b1-116">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="d27b1-117">Stream</span><span class="sxs-lookup"><span data-stu-id="d27b1-117">Stream</span></span>      | <span data-ttu-id="d27b1-118">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="d27b1-118">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="d27b1-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="d27b1-119">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="d27b1-120">Stream</span><span class="sxs-lookup"><span data-stu-id="d27b1-120">Stream</span></span>      | <span data-ttu-id="d27b1-121">Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="d27b1-121">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="d27b1-122">Получение количества пользователей по версиям</span><span class="sxs-lookup"><span data-stu-id="d27b1-122">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="d27b1-123">Поток</span><span class="sxs-lookup"><span data-stu-id="d27b1-123">Stream</span></span>      | <span data-ttu-id="d27b1-124">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="d27b1-124">Get the count of unique users by Outlook desktop version.</span></span> |
