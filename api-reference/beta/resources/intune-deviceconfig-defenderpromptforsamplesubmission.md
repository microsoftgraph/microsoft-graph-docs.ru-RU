---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя для отправки примеров.
author: tfitzmac
ms.openlocfilehash: 19498f587759df56ae671b119b59abe7e7acd62c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314933"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="d8436-103">Тип перечисления defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="d8436-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="d8436-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8436-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8436-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8436-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8436-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d8436-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8436-107">Возможные значения для запроса пользователя для отправки примеров.</span><span class="sxs-lookup"><span data-stu-id="d8436-107">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="d8436-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d8436-108">Members</span></span>
|<span data-ttu-id="d8436-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d8436-109">Member</span></span>|<span data-ttu-id="d8436-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d8436-110">Value</span></span>|<span data-ttu-id="d8436-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8436-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8436-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="d8436-112">userDefined</span></span>|<span data-ttu-id="d8436-113">0</span><span class="sxs-lookup"><span data-stu-id="d8436-113">0</span></span>|<span data-ttu-id="d8436-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="d8436-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d8436-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="d8436-115">alwaysPrompt</span></span>|<span data-ttu-id="d8436-116">1</span><span class="sxs-lookup"><span data-stu-id="d8436-116">1</span></span>|<span data-ttu-id="d8436-117">Всегда запрашивать пользователя.</span><span class="sxs-lookup"><span data-stu-id="d8436-117">Always prompt.</span></span>|
|<span data-ttu-id="d8436-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="d8436-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="d8436-119">2</span><span class="sxs-lookup"><span data-stu-id="d8436-119">2</span></span>|<span data-ttu-id="d8436-120">Запрашивать перед отправкой личных данных.</span><span class="sxs-lookup"><span data-stu-id="d8436-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="d8436-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="d8436-121">neverSendData</span></span>|<span data-ttu-id="d8436-122">3</span><span class="sxs-lookup"><span data-stu-id="d8436-122">3</span></span>|<span data-ttu-id="d8436-123">Никогда не отправлять данные.</span><span class="sxs-lookup"><span data-stu-id="d8436-123">Never send data.</span></span>|
|<span data-ttu-id="d8436-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="d8436-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="d8436-125">4</span><span class="sxs-lookup"><span data-stu-id="d8436-125">4</span></span>|<span data-ttu-id="d8436-126">Отправьте все данные без запроса.</span><span class="sxs-lookup"><span data-stu-id="d8436-126">Send all data without prompting.</span></span>|





