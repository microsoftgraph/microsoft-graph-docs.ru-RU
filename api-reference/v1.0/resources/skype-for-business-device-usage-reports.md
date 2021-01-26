---
title: Отчеты об использовании устройств со Skype для бизнеса
description: Отчеты об использовании устройств со Skype для бизнеса содержат сведения о типах клиентов и устройств, используемых в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: f0e46f94141691a17c5f7636f497c3f03fef71df
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980642"
---
# <a name="skype-for-business-device-usage-reports"></a><span data-ttu-id="4e739-104">Отчеты об использовании устройств со Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="4e739-104">Skype for Business device usage reports</span></span>

<span data-ttu-id="4e739-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e739-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e739-106">Отчеты об использовании устройств со Skype для бизнеса содержат сведения о типах клиентов и устройств, используемых в организации.</span><span class="sxs-lookup"><span data-stu-id="4e739-106">You can use the Skype for Business device usage reports to get details on the types of clients and devices that are used across your organization.</span></span> <span data-ttu-id="4e739-107">Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.</span><span class="sxs-lookup"><span data-stu-id="4e739-107">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="4e739-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 : используемые клиенты Skype для бизнеса.](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)</span><span class="sxs-lookup"><span data-stu-id="4e739-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="reports"></a><span data-ttu-id="4e739-109">Отчеты</span><span class="sxs-lookup"><span data-stu-id="4e739-109">Reports</span></span>

| <span data-ttu-id="4e739-110">Функция</span><span class="sxs-lookup"><span data-stu-id="4e739-110">Function</span></span>                                 | <span data-ttu-id="4e739-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e739-111">Return Type</span></span> | <span data-ttu-id="4e739-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4e739-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="4e739-113">Получение сведений о пользователях</span><span class="sxs-lookup"><span data-stu-id="4e739-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="4e739-114">Stream</span><span class="sxs-lookup"><span data-stu-id="4e739-114">Stream</span></span>      | <span data-ttu-id="4e739-115">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="4e739-115">Get details about Skype for Business device usage by user.</span></span> |
| [<span data-ttu-id="4e739-116">Получение количества пользователей с разбивкой по устройствам</span><span class="sxs-lookup"><span data-stu-id="4e739-116">Get distribution user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="4e739-117">Stream</span><span class="sxs-lookup"><span data-stu-id="4e739-117">Stream</span></span>      | <span data-ttu-id="4e739-118">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="4e739-118">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="4e739-119">В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="4e739-119">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span> |
| [<span data-ttu-id="4e739-120">Получение количества пользователей</span><span class="sxs-lookup"><span data-stu-id="4e739-120">Get user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="4e739-121">Stream</span><span class="sxs-lookup"><span data-stu-id="4e739-121">Stream</span></span>      | <span data-ttu-id="4e739-122">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4e739-122">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="4e739-123">Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="4e739-123">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span> |

