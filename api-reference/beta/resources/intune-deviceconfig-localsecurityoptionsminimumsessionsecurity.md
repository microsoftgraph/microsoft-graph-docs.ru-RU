---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: da31ca3cecc74e1c74270bd34bdad14df35cc1b1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790344"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="041f5-103">тип перечисления Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="041f5-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="041f5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="041f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="041f5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="041f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="041f5-106">Возможные значения для Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="041f5-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="041f5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="041f5-107">Members</span></span>
|<span data-ttu-id="041f5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="041f5-108">Member</span></span>|<span data-ttu-id="041f5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="041f5-109">Value</span></span>|<span data-ttu-id="041f5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="041f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="041f5-111">none</span><span class="sxs-lookup"><span data-stu-id="041f5-111">none</span></span>|<span data-ttu-id="041f5-112">нуль</span><span class="sxs-lookup"><span data-stu-id="041f5-112">0</span></span>|<span data-ttu-id="041f5-113">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="041f5-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="041f5-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="041f5-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="041f5-115">1,1</span><span class="sxs-lookup"><span data-stu-id="041f5-115">1</span></span>|<span data-ttu-id="041f5-116">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="041f5-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="041f5-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="041f5-117">require128BitEncryption</span></span>|<span data-ttu-id="041f5-118">2</span><span class="sxs-lookup"><span data-stu-id="041f5-118">2</span></span>|<span data-ttu-id="041f5-119">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="041f5-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="041f5-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="041f5-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="041f5-121">4</span><span class="sxs-lookup"><span data-stu-id="041f5-121">3</span></span>|<span data-ttu-id="041f5-122">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="041f5-122">Send LM & NTLMv2 responses only</span></span>|



