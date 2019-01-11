---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя для отправки примеров.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f1dbd79d58fa46a4e5e50f989e807763ff10356
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849828"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="f1a15-103">Тип перечисления defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="f1a15-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="f1a15-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1a15-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1a15-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1a15-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1a15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1a15-107">Возможные значения для запроса пользователя для отправки примеров.</span><span class="sxs-lookup"><span data-stu-id="f1a15-107">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="f1a15-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f1a15-108">Members</span></span>
|<span data-ttu-id="f1a15-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f1a15-109">Member</span></span>|<span data-ttu-id="f1a15-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f1a15-110">Value</span></span>|<span data-ttu-id="f1a15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a15-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="f1a15-112">userDefined</span></span>|<span data-ttu-id="f1a15-113">0</span><span class="sxs-lookup"><span data-stu-id="f1a15-113">0</span></span>|<span data-ttu-id="f1a15-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="f1a15-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f1a15-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="f1a15-115">alwaysPrompt</span></span>|<span data-ttu-id="f1a15-116">1</span><span class="sxs-lookup"><span data-stu-id="f1a15-116">1</span></span>|<span data-ttu-id="f1a15-117">Всегда запрашивать пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1a15-117">Always prompt.</span></span>|
|<span data-ttu-id="f1a15-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="f1a15-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="f1a15-119">2</span><span class="sxs-lookup"><span data-stu-id="f1a15-119">2</span></span>|<span data-ttu-id="f1a15-120">Запрашивать перед отправкой личных данных.</span><span class="sxs-lookup"><span data-stu-id="f1a15-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="f1a15-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="f1a15-121">neverSendData</span></span>|<span data-ttu-id="f1a15-122">3</span><span class="sxs-lookup"><span data-stu-id="f1a15-122">3</span></span>|<span data-ttu-id="f1a15-123">Никогда не отправлять данные.</span><span class="sxs-lookup"><span data-stu-id="f1a15-123">Never send data.</span></span>|
|<span data-ttu-id="f1a15-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="f1a15-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="f1a15-125">4</span><span class="sxs-lookup"><span data-stu-id="f1a15-125">4</span></span>|<span data-ttu-id="f1a15-126">Отправьте все данные без запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a15-126">Send all data without prompting.</span></span>|





