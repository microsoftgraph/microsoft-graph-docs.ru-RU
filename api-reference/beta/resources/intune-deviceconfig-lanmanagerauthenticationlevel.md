---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7fd08d1ce3dd40e3c60c8cbc42985f4014e1f332
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269030"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="66f73-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="66f73-103">lanManagerAuthenticationLevel enum type</span></span>

<span data-ttu-id="66f73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66f73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66f73-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66f73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66f73-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66f73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66f73-107">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="66f73-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="66f73-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="66f73-108">Members</span></span>
|<span data-ttu-id="66f73-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="66f73-109">Member</span></span>|<span data-ttu-id="66f73-110">Значение</span><span class="sxs-lookup"><span data-stu-id="66f73-110">Value</span></span>|<span data-ttu-id="66f73-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66f73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66f73-112">лманднлтм</span><span class="sxs-lookup"><span data-stu-id="66f73-112">lmAndNltm</span></span>|<span data-ttu-id="66f73-113">нуль</span><span class="sxs-lookup"><span data-stu-id="66f73-113">0</span></span>|<span data-ttu-id="66f73-114">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="66f73-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="66f73-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="66f73-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="66f73-116">1,1</span><span class="sxs-lookup"><span data-stu-id="66f73-116">1</span></span>|<span data-ttu-id="66f73-117">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="66f73-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="66f73-118">лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="66f73-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="66f73-119">2</span><span class="sxs-lookup"><span data-stu-id="66f73-119">2</span></span>|<span data-ttu-id="66f73-120">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="66f73-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="66f73-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="66f73-121">lmAndNtlmV2</span></span>|<span data-ttu-id="66f73-122">4</span><span class="sxs-lookup"><span data-stu-id="66f73-122">3</span></span>|<span data-ttu-id="66f73-123">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="66f73-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="66f73-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="66f73-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="66f73-125">4 </span><span class="sxs-lookup"><span data-stu-id="66f73-125">4</span></span>|<span data-ttu-id="66f73-126">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="66f73-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="66f73-127">Отклонять LM</span><span class="sxs-lookup"><span data-stu-id="66f73-127">Refuse LM</span></span>|
|<span data-ttu-id="66f73-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="66f73-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="66f73-129">5 </span><span class="sxs-lookup"><span data-stu-id="66f73-129">5</span></span>|<span data-ttu-id="66f73-130">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="66f73-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="66f73-131">Отклонять LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="66f73-131">Refuse LM & NTLM</span></span>|




