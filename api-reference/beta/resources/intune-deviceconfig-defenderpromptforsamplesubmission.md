---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя для отправки примеров.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b706c0086791543a5cbb13d26ae1d86a2e3b1760
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403317"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="da443-103">Тип перечисления defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="da443-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="da443-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da443-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da443-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da443-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da443-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da443-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da443-107">Возможные значения для запроса пользователя для отправки примеров.</span><span class="sxs-lookup"><span data-stu-id="da443-107">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="da443-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="da443-108">Members</span></span>
|<span data-ttu-id="da443-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="da443-109">Member</span></span>|<span data-ttu-id="da443-110">Значение</span><span class="sxs-lookup"><span data-stu-id="da443-110">Value</span></span>|<span data-ttu-id="da443-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da443-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da443-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="da443-112">userDefined</span></span>|<span data-ttu-id="da443-113">0</span><span class="sxs-lookup"><span data-stu-id="da443-113">0</span></span>|<span data-ttu-id="da443-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="da443-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="da443-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="da443-115">alwaysPrompt</span></span>|<span data-ttu-id="da443-116">1</span><span class="sxs-lookup"><span data-stu-id="da443-116">1</span></span>|<span data-ttu-id="da443-117">Всегда запрашивать пользователя.</span><span class="sxs-lookup"><span data-stu-id="da443-117">Always prompt.</span></span>|
|<span data-ttu-id="da443-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="da443-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="da443-119">2</span><span class="sxs-lookup"><span data-stu-id="da443-119">2</span></span>|<span data-ttu-id="da443-120">Запрашивать перед отправкой личных данных.</span><span class="sxs-lookup"><span data-stu-id="da443-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="da443-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="da443-121">neverSendData</span></span>|<span data-ttu-id="da443-122">3</span><span class="sxs-lookup"><span data-stu-id="da443-122">3</span></span>|<span data-ttu-id="da443-123">Никогда не отправлять данные.</span><span class="sxs-lookup"><span data-stu-id="da443-123">Never send data.</span></span>|
|<span data-ttu-id="da443-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="da443-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="da443-125">4</span><span class="sxs-lookup"><span data-stu-id="da443-125">4</span></span>|<span data-ttu-id="da443-126">Отправьте все данные без запроса.</span><span class="sxs-lookup"><span data-stu-id="da443-126">Send all data without prompting.</span></span>|




