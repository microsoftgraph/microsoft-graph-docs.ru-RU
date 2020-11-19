---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 07d284f778dd2cb5bfc9942a649aecbc63ac1b19
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269023"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="22766-103">тип перечисления Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="22766-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="22766-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22766-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22766-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22766-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22766-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22766-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22766-107">Возможные значения для Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="22766-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="22766-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="22766-108">Members</span></span>
|<span data-ttu-id="22766-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="22766-109">Member</span></span>|<span data-ttu-id="22766-110">Значение</span><span class="sxs-lookup"><span data-stu-id="22766-110">Value</span></span>|<span data-ttu-id="22766-111">Описание</span><span class="sxs-lookup"><span data-stu-id="22766-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22766-112">Нет</span><span class="sxs-lookup"><span data-stu-id="22766-112">none</span></span>|<span data-ttu-id="22766-113">нуль</span><span class="sxs-lookup"><span data-stu-id="22766-113">0</span></span>|<span data-ttu-id="22766-114">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="22766-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="22766-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="22766-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="22766-116">1,1</span><span class="sxs-lookup"><span data-stu-id="22766-116">1</span></span>|<span data-ttu-id="22766-117">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="22766-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="22766-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="22766-118">require128BitEncryption</span></span>|<span data-ttu-id="22766-119">2</span><span class="sxs-lookup"><span data-stu-id="22766-119">2</span></span>|<span data-ttu-id="22766-120">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="22766-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="22766-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="22766-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="22766-122">4</span><span class="sxs-lookup"><span data-stu-id="22766-122">3</span></span>|<span data-ttu-id="22766-123">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="22766-123">Send LM & NTLMv2 responses only</span></span>|




