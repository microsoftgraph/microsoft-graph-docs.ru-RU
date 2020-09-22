---
title: Отчеты об использовании устройств со Skype для бизнеса
description: Отчеты об использовании устройств со Skype для бизнеса содержат сведения о типах клиентов и устройств, используемых в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 13eecf37d2389338409cae49493984e38a0cb7b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074841"
---
# <a name="skype-for-business-device-usage-reports"></a><span data-ttu-id="2a9a5-104">Отчеты об использовании устройств со Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="2a9a5-104">Skype for Business device usage reports</span></span>

<span data-ttu-id="2a9a5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a9a5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a9a5-106">Отчеты об использовании устройств со Skype для бизнеса содержат сведения о типах клиентов и устройств, используемых в организации.</span><span class="sxs-lookup"><span data-stu-id="2a9a5-106">You can use the Skype for Business device usage reports to get details on the types of clients and devices that are used across your organization.</span></span> <span data-ttu-id="2a9a5-107">Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.</span><span class="sxs-lookup"><span data-stu-id="2a9a5-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="2a9a5-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="2a9a5-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="reports"></a><span data-ttu-id="2a9a5-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="2a9a5-109">Reports</span></span>

| <span data-ttu-id="2a9a5-110">Функция</span><span class="sxs-lookup"><span data-stu-id="2a9a5-110">Function</span></span>                                 | <span data-ttu-id="2a9a5-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2a9a5-111">Return Type</span></span> | <span data-ttu-id="2a9a5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2a9a5-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="2a9a5-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="2a9a5-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="2a9a5-114">Stream</span><span class="sxs-lookup"><span data-stu-id="2a9a5-114">Stream</span></span>      | <span data-ttu-id="2a9a5-115">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="2a9a5-115">Get details about Skype for Business device usage by user.</span></span> |
| [<span data-ttu-id="2a9a5-116">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="2a9a5-116">Get distribution user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="2a9a5-117">Stream</span><span class="sxs-lookup"><span data-stu-id="2a9a5-117">Stream</span></span>      | <span data-ttu-id="2a9a5-118">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="2a9a5-118">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="2a9a5-119">В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="2a9a5-119">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span> |
| [<span data-ttu-id="2a9a5-120">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="2a9a5-120">Get user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="2a9a5-121">Stream</span><span class="sxs-lookup"><span data-stu-id="2a9a5-121">Stream</span></span>      | <span data-ttu-id="2a9a5-122">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2a9a5-122">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="2a9a5-123">Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="2a9a5-123">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span> |

