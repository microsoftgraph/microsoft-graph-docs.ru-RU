---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac7ebd94f791372b4bd7b74189204a7b8a4d0360
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989296"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="48c0e-103">тип перечисления Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="48c0e-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="48c0e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48c0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48c0e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48c0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48c0e-106">Возможные значения для Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="48c0e-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="48c0e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="48c0e-107">Members</span></span>
|<span data-ttu-id="48c0e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="48c0e-108">Member</span></span>|<span data-ttu-id="48c0e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="48c0e-109">Value</span></span>|<span data-ttu-id="48c0e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="48c0e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48c0e-111">none</span><span class="sxs-lookup"><span data-stu-id="48c0e-111">none</span></span>|<span data-ttu-id="48c0e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="48c0e-112">0</span></span>|<span data-ttu-id="48c0e-113">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="48c0e-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="48c0e-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="48c0e-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="48c0e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="48c0e-115">1</span></span>|<span data-ttu-id="48c0e-116">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="48c0e-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="48c0e-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="48c0e-117">require128BitEncryption</span></span>|<span data-ttu-id="48c0e-118">2</span><span class="sxs-lookup"><span data-stu-id="48c0e-118">2</span></span>|<span data-ttu-id="48c0e-119">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="48c0e-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="48c0e-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="48c0e-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="48c0e-121">4</span><span class="sxs-lookup"><span data-stu-id="48c0e-121">3</span></span>|<span data-ttu-id="48c0e-122">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="48c0e-122">Send LM & NTLMv2 responses only</span></span>|





