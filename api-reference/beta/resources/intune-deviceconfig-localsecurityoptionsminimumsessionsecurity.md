---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4750d5bc4da34f1e627d2b324827f78f830bb219
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526222"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="3999c-103">тип перечисления Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="3999c-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="3999c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3999c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3999c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3999c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3999c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3999c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3999c-107">Возможные значения для Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="3999c-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="3999c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3999c-108">Members</span></span>
|<span data-ttu-id="3999c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3999c-109">Member</span></span>|<span data-ttu-id="3999c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3999c-110">Value</span></span>|<span data-ttu-id="3999c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3999c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3999c-112">нет</span><span class="sxs-lookup"><span data-stu-id="3999c-112">none</span></span>|<span data-ttu-id="3999c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3999c-113">0</span></span>|<span data-ttu-id="3999c-114">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="3999c-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="3999c-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="3999c-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="3999c-116">1 </span><span class="sxs-lookup"><span data-stu-id="3999c-116">1</span></span>|<span data-ttu-id="3999c-117">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="3999c-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="3999c-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="3999c-118">require128BitEncryption</span></span>|<span data-ttu-id="3999c-119">2 </span><span class="sxs-lookup"><span data-stu-id="3999c-119">2</span></span>|<span data-ttu-id="3999c-120">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="3999c-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="3999c-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="3999c-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="3999c-122">3 </span><span class="sxs-lookup"><span data-stu-id="3999c-122">3</span></span>|<span data-ttu-id="3999c-123">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="3999c-123">Send LM & NTLMv2 responses only</span></span>|



