---
title: Тип перечисления lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
ms.openlocfilehash: 9fb8113c4953a0cabcecfbc5303b9f62f685d5ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075279"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="05296-103">Тип перечисления lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="05296-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="05296-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05296-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05296-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05296-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05296-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05296-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05296-107">Возможные значения для LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="05296-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="05296-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="05296-108">Members</span></span>
|<span data-ttu-id="05296-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="05296-109">Member</span></span>|<span data-ttu-id="05296-110">Значение</span><span class="sxs-lookup"><span data-stu-id="05296-110">Value</span></span>|<span data-ttu-id="05296-111">Description</span><span class="sxs-lookup"><span data-stu-id="05296-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05296-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="05296-112">lmAndNltm</span></span>|<span data-ttu-id="05296-113">0</span><span class="sxs-lookup"><span data-stu-id="05296-113">0</span></span>|<span data-ttu-id="05296-114">Отправлять ответы LM и NTLM</span><span class="sxs-lookup"><span data-stu-id="05296-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="05296-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="05296-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="05296-116">1</span><span class="sxs-lookup"><span data-stu-id="05296-116">1</span></span>|<span data-ttu-id="05296-117">Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование</span><span class="sxs-lookup"><span data-stu-id="05296-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="05296-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="05296-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="05296-119">2</span><span class="sxs-lookup"><span data-stu-id="05296-119">2</span></span>|<span data-ttu-id="05296-120">Отправлять LM и NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="05296-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="05296-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="05296-121">lmAndNtlmV2</span></span>|<span data-ttu-id="05296-122">3</span><span class="sxs-lookup"><span data-stu-id="05296-122">3</span></span>|<span data-ttu-id="05296-123">Отправлять LM и NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="05296-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="05296-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="05296-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="05296-125">4</span><span class="sxs-lookup"><span data-stu-id="05296-125">4</span></span>|<span data-ttu-id="05296-126">Отправьте LM и NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="05296-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="05296-127">Отказывать LM</span><span class="sxs-lookup"><span data-stu-id="05296-127">Refuse LM</span></span>|
|<span data-ttu-id="05296-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="05296-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="05296-129">5</span><span class="sxs-lookup"><span data-stu-id="05296-129">5</span></span>|<span data-ttu-id="05296-130">Отправьте LM и NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="05296-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="05296-131">Отказ от LM и NTLM</span><span class="sxs-lookup"><span data-stu-id="05296-131">Refuse LM & NTLM</span></span>|





