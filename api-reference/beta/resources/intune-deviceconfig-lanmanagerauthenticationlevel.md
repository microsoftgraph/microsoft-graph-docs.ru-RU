---
title: Тип перечисления lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68af209a005dc1d7e8d25672f5e97e1d929ba25b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866915"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="416a8-103">Тип перечисления lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="416a8-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="416a8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="416a8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="416a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="416a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="416a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="416a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="416a8-107">Возможные значения для LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="416a8-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="416a8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="416a8-108">Members</span></span>
|<span data-ttu-id="416a8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="416a8-109">Member</span></span>|<span data-ttu-id="416a8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="416a8-110">Value</span></span>|<span data-ttu-id="416a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="416a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="416a8-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="416a8-112">lmAndNltm</span></span>|<span data-ttu-id="416a8-113">0</span><span class="sxs-lookup"><span data-stu-id="416a8-113">0</span></span>|<span data-ttu-id="416a8-114">Отправлять ответы LM и NTLM</span><span class="sxs-lookup"><span data-stu-id="416a8-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="416a8-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="416a8-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="416a8-116">1</span><span class="sxs-lookup"><span data-stu-id="416a8-116">1</span></span>|<span data-ttu-id="416a8-117">Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование</span><span class="sxs-lookup"><span data-stu-id="416a8-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="416a8-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="416a8-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="416a8-119">2</span><span class="sxs-lookup"><span data-stu-id="416a8-119">2</span></span>|<span data-ttu-id="416a8-120">Отправлять LM и NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="416a8-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="416a8-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="416a8-121">lmAndNtlmV2</span></span>|<span data-ttu-id="416a8-122">3</span><span class="sxs-lookup"><span data-stu-id="416a8-122">3</span></span>|<span data-ttu-id="416a8-123">Отправлять LM и NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="416a8-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="416a8-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="416a8-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="416a8-125">4</span><span class="sxs-lookup"><span data-stu-id="416a8-125">4</span></span>|<span data-ttu-id="416a8-126">Отправьте LM и NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="416a8-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="416a8-127">Отказывать LM</span><span class="sxs-lookup"><span data-stu-id="416a8-127">Refuse LM</span></span>|
|<span data-ttu-id="416a8-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="416a8-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="416a8-129">5</span><span class="sxs-lookup"><span data-stu-id="416a8-129">5</span></span>|<span data-ttu-id="416a8-130">Отправьте LM и NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="416a8-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="416a8-131">Отказ от LM и NTLM</span><span class="sxs-lookup"><span data-stu-id="416a8-131">Refuse LM & NTLM</span></span>|





