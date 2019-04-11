---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b93f229661de3e2fbb28f764288983b2fd83bb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801248"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="5e2fb-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="5e2fb-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="5e2fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e2fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e2fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e2fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e2fb-106">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="5e2fb-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="5e2fb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5e2fb-107">Members</span></span>
|<span data-ttu-id="5e2fb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5e2fb-108">Member</span></span>|<span data-ttu-id="5e2fb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5e2fb-109">Value</span></span>|<span data-ttu-id="5e2fb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e2fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e2fb-111">Лманднлтм</span><span class="sxs-lookup"><span data-stu-id="5e2fb-111">lmAndNltm</span></span>|<span data-ttu-id="5e2fb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5e2fb-112">0</span></span>|<span data-ttu-id="5e2fb-113">Отправка ответов LM _Амп_ NTLM</span><span class="sxs-lookup"><span data-stu-id="5e2fb-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="5e2fb-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="5e2fb-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="5e2fb-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5e2fb-115">1</span></span>|<span data-ttu-id="5e2fb-116">Отправлять LM _Амп_ NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="5e2fb-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="5e2fb-117">Лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="5e2fb-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="5e2fb-118">2</span><span class="sxs-lookup"><span data-stu-id="5e2fb-118">2</span></span>|<span data-ttu-id="5e2fb-119">Отправлять только LM _Амп_ NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="5e2fb-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="5e2fb-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="5e2fb-120">lmAndNtlmV2</span></span>|<span data-ttu-id="5e2fb-121">4</span><span class="sxs-lookup"><span data-stu-id="5e2fb-121">3</span></span>|<span data-ttu-id="5e2fb-122">Отправлять только LM _Амп_ NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="5e2fb-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="5e2fb-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="5e2fb-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="5e2fb-124">SP4</span><span class="sxs-lookup"><span data-stu-id="5e2fb-124">4</span></span>|<span data-ttu-id="5e2fb-125">Отправлять только ответы LM _Амп_ NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="5e2fb-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="5e2fb-126">ОтКлонять LM</span><span class="sxs-lookup"><span data-stu-id="5e2fb-126">Refuse LM</span></span>|
|<span data-ttu-id="5e2fb-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="5e2fb-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="5e2fb-128">17:00</span><span class="sxs-lookup"><span data-stu-id="5e2fb-128">5</span></span>|<span data-ttu-id="5e2fb-129">Отправлять только ответы LM _Амп_ NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="5e2fb-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="5e2fb-130">ОтКлонять LM _Амп_ NTLM</span><span class="sxs-lookup"><span data-stu-id="5e2fb-130">Refuse LM & NTLM</span></span>|





