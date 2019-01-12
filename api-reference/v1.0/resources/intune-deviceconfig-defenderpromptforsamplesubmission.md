---
title: Тип перечисления defenderPromptForSampleSubmission
description: Возможные значения для запроса пользователя для отправки примеров.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e103916bd55e6c2d505a85c379b80962ab9a0cac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928089"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="8aa56-103">Тип перечисления defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="8aa56-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="8aa56-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8aa56-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8aa56-105">Возможные значения для запроса пользователя для отправки примеров.</span><span class="sxs-lookup"><span data-stu-id="8aa56-105">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="8aa56-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="8aa56-106">Members</span></span>
|<span data-ttu-id="8aa56-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="8aa56-107">Member</span></span>|<span data-ttu-id="8aa56-108">Значение</span><span class="sxs-lookup"><span data-stu-id="8aa56-108">Value</span></span>|<span data-ttu-id="8aa56-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8aa56-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aa56-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="8aa56-110">userDefined</span></span>|<span data-ttu-id="8aa56-111">0</span><span class="sxs-lookup"><span data-stu-id="8aa56-111">0</span></span>|<span data-ttu-id="8aa56-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="8aa56-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="8aa56-113">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="8aa56-113">alwaysPrompt</span></span>|<span data-ttu-id="8aa56-114">1</span><span class="sxs-lookup"><span data-stu-id="8aa56-114">1</span></span>|<span data-ttu-id="8aa56-115">Всегда запрашивать пользователя.</span><span class="sxs-lookup"><span data-stu-id="8aa56-115">Always prompt.</span></span>|
|<span data-ttu-id="8aa56-116">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="8aa56-116">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="8aa56-117">2</span><span class="sxs-lookup"><span data-stu-id="8aa56-117">2</span></span>|<span data-ttu-id="8aa56-118">Запрашивать перед отправкой личных данных.</span><span class="sxs-lookup"><span data-stu-id="8aa56-118">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="8aa56-119">neverSendData</span><span class="sxs-lookup"><span data-stu-id="8aa56-119">neverSendData</span></span>|<span data-ttu-id="8aa56-120">3</span><span class="sxs-lookup"><span data-stu-id="8aa56-120">3</span></span>|<span data-ttu-id="8aa56-121">Никогда не отправлять данные.</span><span class="sxs-lookup"><span data-stu-id="8aa56-121">Never send data.</span></span>|
|<span data-ttu-id="8aa56-122">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="8aa56-122">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="8aa56-123">4</span><span class="sxs-lookup"><span data-stu-id="8aa56-123">4</span></span>|<span data-ttu-id="8aa56-124">Отправьте все данные без запроса.</span><span class="sxs-lookup"><span data-stu-id="8aa56-124">Send all data without prompting.</span></span>|



