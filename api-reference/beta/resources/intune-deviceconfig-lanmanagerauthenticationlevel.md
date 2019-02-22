---
title: тип перечисления Ланманажераусентикатионлевел
description: Возможные значения для Ланманажераусентикатионлевел
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f04f1ef2fc12fa0352aeec803c46fb4ebab3d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166572"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="273d5-103">тип перечисления Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="273d5-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="273d5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="273d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="273d5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="273d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="273d5-106">Возможные значения для Ланманажераусентикатионлевел</span><span class="sxs-lookup"><span data-stu-id="273d5-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="273d5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="273d5-107">Members</span></span>
|<span data-ttu-id="273d5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="273d5-108">Member</span></span>|<span data-ttu-id="273d5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="273d5-109">Value</span></span>|<span data-ttu-id="273d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="273d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="273d5-111">Лманднлтм</span><span class="sxs-lookup"><span data-stu-id="273d5-111">lmAndNltm</span></span>|<span data-ttu-id="273d5-112">нуль</span><span class="sxs-lookup"><span data-stu-id="273d5-112">0</span></span>|<span data-ttu-id="273d5-113">Отправка ответов LM _Амп_ NTLM</span><span class="sxs-lookup"><span data-stu-id="273d5-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="273d5-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="273d5-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="273d5-115">1,1</span><span class="sxs-lookup"><span data-stu-id="273d5-115">1</span></span>|<span data-ttu-id="273d5-116">Отправлять LM _Амп_ NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="273d5-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="273d5-117">Лманднтлмонли</span><span class="sxs-lookup"><span data-stu-id="273d5-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="273d5-118">2</span><span class="sxs-lookup"><span data-stu-id="273d5-118">2</span></span>|<span data-ttu-id="273d5-119">Отправлять только LM _Амп_ NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="273d5-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="273d5-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="273d5-120">lmAndNtlmV2</span></span>|<span data-ttu-id="273d5-121">4</span><span class="sxs-lookup"><span data-stu-id="273d5-121">3</span></span>|<span data-ttu-id="273d5-122">Отправлять только LM _Амп_ NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="273d5-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="273d5-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="273d5-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="273d5-124">4</span><span class="sxs-lookup"><span data-stu-id="273d5-124">4</span></span>|<span data-ttu-id="273d5-125">Отправлять только ответы LM _Амп_ NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="273d5-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="273d5-126">ОтКлонять LM</span><span class="sxs-lookup"><span data-stu-id="273d5-126">Refuse LM</span></span>|
|<span data-ttu-id="273d5-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="273d5-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="273d5-128">17:00</span><span class="sxs-lookup"><span data-stu-id="273d5-128">5</span></span>|<span data-ttu-id="273d5-129">Отправлять только ответы LM _Амп_ NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="273d5-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="273d5-130">ОтКлонять LM _Амп_ NTLM</span><span class="sxs-lookup"><span data-stu-id="273d5-130">Refuse LM & NTLM</span></span>|




