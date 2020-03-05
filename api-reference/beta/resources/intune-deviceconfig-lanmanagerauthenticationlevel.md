---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8b979c66469ac29339045dd9d1341f85839084bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529762"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="2e8a6-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="2e8a6-103">lanManagerAuthenticationLevel enum type</span></span>

<span data-ttu-id="2e8a6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2e8a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e8a6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e8a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e8a6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e8a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e8a6-107">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="2e8a6-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="2e8a6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2e8a6-108">Members</span></span>
|<span data-ttu-id="2e8a6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2e8a6-109">Member</span></span>|<span data-ttu-id="2e8a6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2e8a6-110">Value</span></span>|<span data-ttu-id="2e8a6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2e8a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e8a6-112">лманднлтм</span><span class="sxs-lookup"><span data-stu-id="2e8a6-112">lmAndNltm</span></span>|<span data-ttu-id="2e8a6-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2e8a6-113">0</span></span>|<span data-ttu-id="2e8a6-114">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="2e8a6-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="2e8a6-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="2e8a6-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="2e8a6-116">1 </span><span class="sxs-lookup"><span data-stu-id="2e8a6-116">1</span></span>|<span data-ttu-id="2e8a6-117">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="2e8a6-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="2e8a6-118">лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="2e8a6-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="2e8a6-119">2 </span><span class="sxs-lookup"><span data-stu-id="2e8a6-119">2</span></span>|<span data-ttu-id="2e8a6-120">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="2e8a6-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="2e8a6-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="2e8a6-121">lmAndNtlmV2</span></span>|<span data-ttu-id="2e8a6-122">3 </span><span class="sxs-lookup"><span data-stu-id="2e8a6-122">3</span></span>|<span data-ttu-id="2e8a6-123">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="2e8a6-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="2e8a6-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="2e8a6-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="2e8a6-125">4 </span><span class="sxs-lookup"><span data-stu-id="2e8a6-125">4</span></span>|<span data-ttu-id="2e8a6-126">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="2e8a6-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="2e8a6-127">Отклонять LM</span><span class="sxs-lookup"><span data-stu-id="2e8a6-127">Refuse LM</span></span>|
|<span data-ttu-id="2e8a6-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="2e8a6-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="2e8a6-129">5 </span><span class="sxs-lookup"><span data-stu-id="2e8a6-129">5</span></span>|<span data-ttu-id="2e8a6-130">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="2e8a6-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="2e8a6-131">Отклонять LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="2e8a6-131">Refuse LM & NTLM</span></span>|



