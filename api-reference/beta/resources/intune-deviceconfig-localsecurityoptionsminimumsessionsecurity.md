---
title: тип перечисления Локалсекуритйоптионсминимумсессионсекурити
description: Возможные значения для Локалсекуритйоптионсминимумсессионсекурити
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f5d7e052d5b814bb10d3c0851683deccdf9f9f5f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439975"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="73f0d-103">тип перечисления Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="73f0d-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="73f0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73f0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73f0d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73f0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73f0d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73f0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73f0d-107">Возможные значения для Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="73f0d-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="73f0d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="73f0d-108">Members</span></span>
|<span data-ttu-id="73f0d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="73f0d-109">Member</span></span>|<span data-ttu-id="73f0d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="73f0d-110">Value</span></span>|<span data-ttu-id="73f0d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="73f0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73f0d-112">нет</span><span class="sxs-lookup"><span data-stu-id="73f0d-112">none</span></span>|<span data-ttu-id="73f0d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="73f0d-113">0</span></span>|<span data-ttu-id="73f0d-114">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="73f0d-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="73f0d-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="73f0d-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="73f0d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="73f0d-116">1</span></span>|<span data-ttu-id="73f0d-117">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="73f0d-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="73f0d-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="73f0d-118">require128BitEncryption</span></span>|<span data-ttu-id="73f0d-119">2</span><span class="sxs-lookup"><span data-stu-id="73f0d-119">2</span></span>|<span data-ttu-id="73f0d-120">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="73f0d-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="73f0d-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="73f0d-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="73f0d-122">4</span><span class="sxs-lookup"><span data-stu-id="73f0d-122">3</span></span>|<span data-ttu-id="73f0d-123">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="73f0d-123">Send LM & NTLMv2 responses only</span></span>|



