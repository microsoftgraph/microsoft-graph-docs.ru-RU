---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8dc6a96f5dda3cdba9ea3a57507bef4f32edc5a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325528"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="e5a9e-103">тип перечисления Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="e5a9e-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="e5a9e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5a9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5a9e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5a9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5a9e-106">Возможные значения для Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="e5a9e-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="e5a9e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e5a9e-107">Members</span></span>
|<span data-ttu-id="e5a9e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e5a9e-108">Member</span></span>|<span data-ttu-id="e5a9e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e5a9e-109">Value</span></span>|<span data-ttu-id="e5a9e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e5a9e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5a9e-111">none</span><span class="sxs-lookup"><span data-stu-id="e5a9e-111">none</span></span>|<span data-ttu-id="e5a9e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e5a9e-112">0</span></span>|<span data-ttu-id="e5a9e-113">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="e5a9e-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="e5a9e-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="e5a9e-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="e5a9e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e5a9e-115">1</span></span>|<span data-ttu-id="e5a9e-116">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="e5a9e-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="e5a9e-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="e5a9e-117">require128BitEncryption</span></span>|<span data-ttu-id="e5a9e-118">2</span><span class="sxs-lookup"><span data-stu-id="e5a9e-118">2</span></span>|<span data-ttu-id="e5a9e-119">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="e5a9e-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="e5a9e-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="e5a9e-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="e5a9e-121">4</span><span class="sxs-lookup"><span data-stu-id="e5a9e-121">3</span></span>|<span data-ttu-id="e5a9e-122">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="e5a9e-122">Send LM & NTLMv2 responses only</span></span>|



