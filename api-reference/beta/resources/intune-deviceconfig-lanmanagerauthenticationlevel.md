---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9516b2b315decf66a85adf6592bc9af00c1dbfa9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439871"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="cc125-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="cc125-103">lanManagerAuthenticationLevel enum type</span></span>

<span data-ttu-id="cc125-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc125-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc125-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc125-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc125-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc125-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc125-107">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="cc125-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="cc125-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="cc125-108">Members</span></span>
|<span data-ttu-id="cc125-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="cc125-109">Member</span></span>|<span data-ttu-id="cc125-110">Значение</span><span class="sxs-lookup"><span data-stu-id="cc125-110">Value</span></span>|<span data-ttu-id="cc125-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc125-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc125-112">лманднлтм</span><span class="sxs-lookup"><span data-stu-id="cc125-112">lmAndNltm</span></span>|<span data-ttu-id="cc125-113">нуль</span><span class="sxs-lookup"><span data-stu-id="cc125-113">0</span></span>|<span data-ttu-id="cc125-114">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="cc125-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="cc125-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="cc125-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="cc125-116">1,1</span><span class="sxs-lookup"><span data-stu-id="cc125-116">1</span></span>|<span data-ttu-id="cc125-117">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="cc125-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="cc125-118">лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="cc125-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="cc125-119">2</span><span class="sxs-lookup"><span data-stu-id="cc125-119">2</span></span>|<span data-ttu-id="cc125-120">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="cc125-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="cc125-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="cc125-121">lmAndNtlmV2</span></span>|<span data-ttu-id="cc125-122">4</span><span class="sxs-lookup"><span data-stu-id="cc125-122">3</span></span>|<span data-ttu-id="cc125-123">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="cc125-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="cc125-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="cc125-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="cc125-125">4 </span><span class="sxs-lookup"><span data-stu-id="cc125-125">4</span></span>|<span data-ttu-id="cc125-126">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="cc125-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="cc125-127">Отклонять LM</span><span class="sxs-lookup"><span data-stu-id="cc125-127">Refuse LM</span></span>|
|<span data-ttu-id="cc125-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="cc125-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="cc125-129">5 </span><span class="sxs-lookup"><span data-stu-id="cc125-129">5</span></span>|<span data-ttu-id="cc125-130">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="cc125-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="cc125-131">Отклонять LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="cc125-131">Refuse LM & NTLM</span></span>|



