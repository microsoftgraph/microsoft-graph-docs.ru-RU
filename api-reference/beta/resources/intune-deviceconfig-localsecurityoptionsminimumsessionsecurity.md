---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ab015e80b276870e663d47a3b8b18d17fed82a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946170"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="7f111-103">тип перечисления Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="7f111-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="7f111-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f111-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f111-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f111-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f111-106">Возможные значения для Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="7f111-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="7f111-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7f111-107">Members</span></span>
|<span data-ttu-id="7f111-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7f111-108">Member</span></span>|<span data-ttu-id="7f111-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7f111-109">Value</span></span>|<span data-ttu-id="7f111-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f111-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f111-111">none</span><span class="sxs-lookup"><span data-stu-id="7f111-111">none</span></span>|<span data-ttu-id="7f111-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7f111-112">0</span></span>|<span data-ttu-id="7f111-113">Отправка ответов LM _Амп_ NTLM</span><span class="sxs-lookup"><span data-stu-id="7f111-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="7f111-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="7f111-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="7f111-115">1,1</span><span class="sxs-lookup"><span data-stu-id="7f111-115">1</span></span>|<span data-ttu-id="7f111-116">Отправлять LM _Амп_ NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="7f111-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="7f111-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="7f111-117">require128BitEncryption</span></span>|<span data-ttu-id="7f111-118">2</span><span class="sxs-lookup"><span data-stu-id="7f111-118">2</span></span>|<span data-ttu-id="7f111-119">Отправлять только LM _Амп_ NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="7f111-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="7f111-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="7f111-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="7f111-121">4</span><span class="sxs-lookup"><span data-stu-id="7f111-121">3</span></span>|<span data-ttu-id="7f111-122">Отправлять только LM _Амп_ NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="7f111-122">Send LM & NTLMv2 responses only</span></span>|




