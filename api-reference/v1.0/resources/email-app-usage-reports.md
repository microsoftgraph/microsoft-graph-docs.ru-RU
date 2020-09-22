---
title: Отчеты об использовании почтовых приложений
description: Эти отчеты позволяют узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 18403a0040672c2c056b9cc03246e29a91639e45
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069129"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="94b13-104">Отчеты об использовании почтовых приложений</span><span class="sxs-lookup"><span data-stu-id="94b13-104">Email app usage reports</span></span>

<span data-ttu-id="94b13-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94b13-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94b13-106">Эти отчеты позволяют узнать, сколько почтовых приложений используется для подключения к Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="94b13-106">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="94b13-107">Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.</span><span class="sxs-lookup"><span data-stu-id="94b13-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="94b13-108">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="94b13-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="94b13-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="94b13-109">Reports</span></span>

| <span data-ttu-id="94b13-110">Функция</span><span class="sxs-lookup"><span data-stu-id="94b13-110">Function</span></span>                                 | <span data-ttu-id="94b13-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="94b13-111">Return Type</span></span> | <span data-ttu-id="94b13-112">Описание</span><span class="sxs-lookup"><span data-stu-id="94b13-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="94b13-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="94b13-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="94b13-114">Stream</span><span class="sxs-lookup"><span data-stu-id="94b13-114">Stream</span></span>      | <span data-ttu-id="94b13-115">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="94b13-115">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="94b13-116">Получение количества пользователей по приложениям</span><span class="sxs-lookup"><span data-stu-id="94b13-116">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="94b13-117">Поток</span><span class="sxs-lookup"><span data-stu-id="94b13-117">Stream</span></span>      | <span data-ttu-id="94b13-118">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="94b13-118">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="94b13-119">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="94b13-119">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="94b13-120">Stream</span><span class="sxs-lookup"><span data-stu-id="94b13-120">Stream</span></span>      | <span data-ttu-id="94b13-121">Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="94b13-121">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="94b13-122">Получение количества пользователей по версиям</span><span class="sxs-lookup"><span data-stu-id="94b13-122">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="94b13-123">Поток</span><span class="sxs-lookup"><span data-stu-id="94b13-123">Stream</span></span>      | <span data-ttu-id="94b13-124">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="94b13-124">Get the count of unique users by Outlook desktop version.</span></span> |

