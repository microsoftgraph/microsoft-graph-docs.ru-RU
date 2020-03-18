---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 670cb0bec6915b79102eae227a261f26eb052413
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790379"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="24370-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="24370-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="24370-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24370-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24370-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24370-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24370-106">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="24370-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="24370-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="24370-107">Members</span></span>
|<span data-ttu-id="24370-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="24370-108">Member</span></span>|<span data-ttu-id="24370-109">Значение</span><span class="sxs-lookup"><span data-stu-id="24370-109">Value</span></span>|<span data-ttu-id="24370-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24370-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24370-111">лманднлтм</span><span class="sxs-lookup"><span data-stu-id="24370-111">lmAndNltm</span></span>|<span data-ttu-id="24370-112">нуль</span><span class="sxs-lookup"><span data-stu-id="24370-112">0</span></span>|<span data-ttu-id="24370-113">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="24370-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="24370-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="24370-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="24370-115">1,1</span><span class="sxs-lookup"><span data-stu-id="24370-115">1</span></span>|<span data-ttu-id="24370-116">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="24370-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="24370-117">лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="24370-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="24370-118">2</span><span class="sxs-lookup"><span data-stu-id="24370-118">2</span></span>|<span data-ttu-id="24370-119">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="24370-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="24370-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="24370-120">lmAndNtlmV2</span></span>|<span data-ttu-id="24370-121">4</span><span class="sxs-lookup"><span data-stu-id="24370-121">3</span></span>|<span data-ttu-id="24370-122">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="24370-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="24370-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="24370-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="24370-124">4 </span><span class="sxs-lookup"><span data-stu-id="24370-124">4</span></span>|<span data-ttu-id="24370-125">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="24370-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="24370-126">Отклонять LM</span><span class="sxs-lookup"><span data-stu-id="24370-126">Refuse LM</span></span>|
|<span data-ttu-id="24370-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="24370-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="24370-128">5 </span><span class="sxs-lookup"><span data-stu-id="24370-128">5</span></span>|<span data-ttu-id="24370-129">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="24370-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="24370-130">Отклонять LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="24370-130">Refuse LM & NTLM</span></span>|



