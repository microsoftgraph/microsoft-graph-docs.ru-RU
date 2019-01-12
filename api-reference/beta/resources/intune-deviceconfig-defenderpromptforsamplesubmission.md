---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя для отправки примеров.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8dfc1a3aeb80a22041f799fb40ff9b2cc6e3870b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924827"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="dc445-103">Тип перечисления defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="dc445-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="dc445-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc445-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc445-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc445-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc445-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc445-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc445-107">Возможные значения для запроса пользователя для отправки примеров.</span><span class="sxs-lookup"><span data-stu-id="dc445-107">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="dc445-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dc445-108">Members</span></span>
|<span data-ttu-id="dc445-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dc445-109">Member</span></span>|<span data-ttu-id="dc445-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dc445-110">Value</span></span>|<span data-ttu-id="dc445-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc445-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc445-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="dc445-112">userDefined</span></span>|<span data-ttu-id="dc445-113">0</span><span class="sxs-lookup"><span data-stu-id="dc445-113">0</span></span>|<span data-ttu-id="dc445-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="dc445-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="dc445-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="dc445-115">alwaysPrompt</span></span>|<span data-ttu-id="dc445-116">1</span><span class="sxs-lookup"><span data-stu-id="dc445-116">1</span></span>|<span data-ttu-id="dc445-117">Всегда запрашивать пользователя.</span><span class="sxs-lookup"><span data-stu-id="dc445-117">Always prompt.</span></span>|
|<span data-ttu-id="dc445-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="dc445-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="dc445-119">2</span><span class="sxs-lookup"><span data-stu-id="dc445-119">2</span></span>|<span data-ttu-id="dc445-120">Запрашивать перед отправкой личных данных.</span><span class="sxs-lookup"><span data-stu-id="dc445-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="dc445-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="dc445-121">neverSendData</span></span>|<span data-ttu-id="dc445-122">3</span><span class="sxs-lookup"><span data-stu-id="dc445-122">3</span></span>|<span data-ttu-id="dc445-123">Никогда не отправлять данные.</span><span class="sxs-lookup"><span data-stu-id="dc445-123">Never send data.</span></span>|
|<span data-ttu-id="dc445-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="dc445-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="dc445-125">4</span><span class="sxs-lookup"><span data-stu-id="dc445-125">4</span></span>|<span data-ttu-id="dc445-126">Отправьте все данные без запроса.</span><span class="sxs-lookup"><span data-stu-id="dc445-126">Send all data without prompting.</span></span>|





