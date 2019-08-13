---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ade139765c9a362cd0c9f9365af0026c51ecb4ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356727"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="ad18e-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="ad18e-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="ad18e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad18e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad18e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad18e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad18e-106">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="ad18e-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="ad18e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ad18e-107">Members</span></span>
|<span data-ttu-id="ad18e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ad18e-108">Member</span></span>|<span data-ttu-id="ad18e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ad18e-109">Value</span></span>|<span data-ttu-id="ad18e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad18e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad18e-111">лманднлтм</span><span class="sxs-lookup"><span data-stu-id="ad18e-111">lmAndNltm</span></span>|<span data-ttu-id="ad18e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ad18e-112">0</span></span>|<span data-ttu-id="ad18e-113">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="ad18e-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="ad18e-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="ad18e-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="ad18e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ad18e-115">1</span></span>|<span data-ttu-id="ad18e-116">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="ad18e-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="ad18e-117">лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="ad18e-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="ad18e-118">2</span><span class="sxs-lookup"><span data-stu-id="ad18e-118">2</span></span>|<span data-ttu-id="ad18e-119">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="ad18e-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="ad18e-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="ad18e-120">lmAndNtlmV2</span></span>|<span data-ttu-id="ad18e-121">4</span><span class="sxs-lookup"><span data-stu-id="ad18e-121">3</span></span>|<span data-ttu-id="ad18e-122">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="ad18e-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="ad18e-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="ad18e-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="ad18e-124">SP4</span><span class="sxs-lookup"><span data-stu-id="ad18e-124">4</span></span>|<span data-ttu-id="ad18e-125">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="ad18e-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="ad18e-126">Отклонять LM</span><span class="sxs-lookup"><span data-stu-id="ad18e-126">Refuse LM</span></span>|
|<span data-ttu-id="ad18e-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="ad18e-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="ad18e-128">17:00</span><span class="sxs-lookup"><span data-stu-id="ad18e-128">5</span></span>|<span data-ttu-id="ad18e-129">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="ad18e-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="ad18e-130">Отклонять LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="ad18e-130">Refuse LM & NTLM</span></span>|



