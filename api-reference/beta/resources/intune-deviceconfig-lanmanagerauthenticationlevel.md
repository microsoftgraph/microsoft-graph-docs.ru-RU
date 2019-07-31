---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f76a0b685a0759a4455d8de805424ddd09758a63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970285"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="c67b6-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="c67b6-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="c67b6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c67b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c67b6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c67b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c67b6-106">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="c67b6-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="c67b6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c67b6-107">Members</span></span>
|<span data-ttu-id="c67b6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c67b6-108">Member</span></span>|<span data-ttu-id="c67b6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c67b6-109">Value</span></span>|<span data-ttu-id="c67b6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c67b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c67b6-111">Лманднлтм</span><span class="sxs-lookup"><span data-stu-id="c67b6-111">lmAndNltm</span></span>|<span data-ttu-id="c67b6-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c67b6-112">0</span></span>|<span data-ttu-id="c67b6-113">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="c67b6-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="c67b6-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="c67b6-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="c67b6-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c67b6-115">1</span></span>|<span data-ttu-id="c67b6-116">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="c67b6-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="c67b6-117">Лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="c67b6-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="c67b6-118">2</span><span class="sxs-lookup"><span data-stu-id="c67b6-118">2</span></span>|<span data-ttu-id="c67b6-119">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="c67b6-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="c67b6-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="c67b6-120">lmAndNtlmV2</span></span>|<span data-ttu-id="c67b6-121">4</span><span class="sxs-lookup"><span data-stu-id="c67b6-121">3</span></span>|<span data-ttu-id="c67b6-122">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="c67b6-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="c67b6-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="c67b6-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="c67b6-124">SP4</span><span class="sxs-lookup"><span data-stu-id="c67b6-124">4</span></span>|<span data-ttu-id="c67b6-125">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="c67b6-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="c67b6-126">Отклонять LM</span><span class="sxs-lookup"><span data-stu-id="c67b6-126">Refuse LM</span></span>|
|<span data-ttu-id="c67b6-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="c67b6-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="c67b6-128">17:00</span><span class="sxs-lookup"><span data-stu-id="c67b6-128">5</span></span>|<span data-ttu-id="c67b6-129">Отправлять только LM & NTLMv2 ответы.</span><span class="sxs-lookup"><span data-stu-id="c67b6-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="c67b6-130">Отклонять LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="c67b6-130">Refuse LM & NTLM</span></span>|





