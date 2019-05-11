---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92cb5b32d8b4768af63d92461597c32f858c0a7c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946156"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="fb7ae-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="fb7ae-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="fb7ae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb7ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb7ae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb7ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb7ae-106">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="fb7ae-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="fb7ae-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="fb7ae-107">Members</span></span>
|<span data-ttu-id="fb7ae-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="fb7ae-108">Member</span></span>|<span data-ttu-id="fb7ae-109">Значение</span><span class="sxs-lookup"><span data-stu-id="fb7ae-109">Value</span></span>|<span data-ttu-id="fb7ae-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb7ae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb7ae-111">Лманднлтм</span><span class="sxs-lookup"><span data-stu-id="fb7ae-111">lmAndNltm</span></span>|<span data-ttu-id="fb7ae-112">нуль</span><span class="sxs-lookup"><span data-stu-id="fb7ae-112">0</span></span>|<span data-ttu-id="fb7ae-113">Отправка ответов LM _Амп_ NTLM</span><span class="sxs-lookup"><span data-stu-id="fb7ae-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="fb7ae-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="fb7ae-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="fb7ae-115">1,1</span><span class="sxs-lookup"><span data-stu-id="fb7ae-115">1</span></span>|<span data-ttu-id="fb7ae-116">Отправлять LM _Амп_ NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="fb7ae-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="fb7ae-117">Лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="fb7ae-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="fb7ae-118">2</span><span class="sxs-lookup"><span data-stu-id="fb7ae-118">2</span></span>|<span data-ttu-id="fb7ae-119">Отправлять только LM _Амп_ NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="fb7ae-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="fb7ae-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="fb7ae-120">lmAndNtlmV2</span></span>|<span data-ttu-id="fb7ae-121">4</span><span class="sxs-lookup"><span data-stu-id="fb7ae-121">3</span></span>|<span data-ttu-id="fb7ae-122">Отправлять только LM _Амп_ NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="fb7ae-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="fb7ae-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="fb7ae-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="fb7ae-124">SP4</span><span class="sxs-lookup"><span data-stu-id="fb7ae-124">4</span></span>|<span data-ttu-id="fb7ae-125">Отправлять только ответы LM _Амп_ NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="fb7ae-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="fb7ae-126">Отклонять LM</span><span class="sxs-lookup"><span data-stu-id="fb7ae-126">Refuse LM</span></span>|
|<span data-ttu-id="fb7ae-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="fb7ae-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="fb7ae-128">17:00</span><span class="sxs-lookup"><span data-stu-id="fb7ae-128">5</span></span>|<span data-ttu-id="fb7ae-129">Отправлять только ответы LM _Амп_ NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="fb7ae-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="fb7ae-130">Отклонять LM _Амп_ NTLM</span><span class="sxs-lookup"><span data-stu-id="fb7ae-130">Refuse LM & NTLM</span></span>|




