---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b71f045ac937af455da428b98242f9d074b14840
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732539"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="2cd9d-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="2cd9d-103">lanManagerAuthenticationLevel enum type</span></span>

<span data-ttu-id="2cd9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cd9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cd9d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cd9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cd9d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cd9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cd9d-107">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="2cd9d-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="2cd9d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2cd9d-108">Members</span></span>
|<span data-ttu-id="2cd9d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2cd9d-109">Member</span></span>|<span data-ttu-id="2cd9d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2cd9d-110">Value</span></span>|<span data-ttu-id="2cd9d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2cd9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd9d-112">лманднлтм</span><span class="sxs-lookup"><span data-stu-id="2cd9d-112">lmAndNltm</span></span>|<span data-ttu-id="2cd9d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2cd9d-113">0</span></span>|<span data-ttu-id="2cd9d-114">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="2cd9d-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="2cd9d-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="2cd9d-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="2cd9d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="2cd9d-116">1</span></span>|<span data-ttu-id="2cd9d-117">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="2cd9d-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="2cd9d-118">лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="2cd9d-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="2cd9d-119">2</span><span class="sxs-lookup"><span data-stu-id="2cd9d-119">2</span></span>|<span data-ttu-id="2cd9d-120">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="2cd9d-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="2cd9d-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="2cd9d-121">lmAndNtlmV2</span></span>|<span data-ttu-id="2cd9d-122">4</span><span class="sxs-lookup"><span data-stu-id="2cd9d-122">3</span></span>|<span data-ttu-id="2cd9d-123">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="2cd9d-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="2cd9d-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="2cd9d-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="2cd9d-125">4 </span><span class="sxs-lookup"><span data-stu-id="2cd9d-125">4</span></span>|<span data-ttu-id="2cd9d-126">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="2cd9d-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="2cd9d-127">Отклонять LM</span><span class="sxs-lookup"><span data-stu-id="2cd9d-127">Refuse LM</span></span>|
|<span data-ttu-id="2cd9d-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="2cd9d-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="2cd9d-129">5 </span><span class="sxs-lookup"><span data-stu-id="2cd9d-129">5</span></span>|<span data-ttu-id="2cd9d-130">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="2cd9d-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="2cd9d-131">Отклонять LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="2cd9d-131">Refuse LM & NTLM</span></span>|





