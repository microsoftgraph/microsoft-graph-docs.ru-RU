---
title: Тип перечисления lanManagerAuthenticationLevel
description: Возможные значения для LanManagerAuthenticationLevel
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397458"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="eef16-103">Тип перечисления lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="eef16-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="eef16-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eef16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eef16-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eef16-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eef16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eef16-107">Возможные значения для LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="eef16-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="eef16-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="eef16-108">Members</span></span>
|<span data-ttu-id="eef16-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="eef16-109">Member</span></span>|<span data-ttu-id="eef16-110">Значение</span><span class="sxs-lookup"><span data-stu-id="eef16-110">Value</span></span>|<span data-ttu-id="eef16-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eef16-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef16-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="eef16-112">lmAndNltm</span></span>|<span data-ttu-id="eef16-113">0</span><span class="sxs-lookup"><span data-stu-id="eef16-113">0</span></span>|<span data-ttu-id="eef16-114">Отправить LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="eef16-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="eef16-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="eef16-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="eef16-116">1</span><span class="sxs-lookup"><span data-stu-id="eef16-116">1</span></span>|<span data-ttu-id="eef16-117">Отправлять LM & использование NTLM сеансовая безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="eef16-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="eef16-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="eef16-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="eef16-119">2</span><span class="sxs-lookup"><span data-stu-id="eef16-119">2</span></span>|<span data-ttu-id="eef16-120">Отправлять LM & только NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="eef16-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="eef16-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="eef16-121">lmAndNtlmV2</span></span>|<span data-ttu-id="eef16-122">3</span><span class="sxs-lookup"><span data-stu-id="eef16-122">3</span></span>|<span data-ttu-id="eef16-123">Отправлять LM & только ответы NTLMv2</span><span class="sxs-lookup"><span data-stu-id="eef16-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="eef16-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="eef16-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="eef16-125">4</span><span class="sxs-lookup"><span data-stu-id="eef16-125">4</span></span>|<span data-ttu-id="eef16-126">Отправьте LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="eef16-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="eef16-127">Отказывать LM</span><span class="sxs-lookup"><span data-stu-id="eef16-127">Refuse LM</span></span>|
|<span data-ttu-id="eef16-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="eef16-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="eef16-129">5</span><span class="sxs-lookup"><span data-stu-id="eef16-129">5</span></span>|<span data-ttu-id="eef16-130">Отправьте LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="eef16-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="eef16-131">Отказ от LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="eef16-131">Refuse LM & NTLM</span></span>|




