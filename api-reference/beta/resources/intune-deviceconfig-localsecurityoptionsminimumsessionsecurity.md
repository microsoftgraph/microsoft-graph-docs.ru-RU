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
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="4d152-103">тип перечисления Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="4d152-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

<span data-ttu-id="4d152-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d152-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d152-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d152-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d152-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d152-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d152-107">Возможные значения для Локалсекуритйоптионсминимумсессионсекурити</span><span class="sxs-lookup"><span data-stu-id="4d152-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="4d152-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4d152-108">Members</span></span>
|<span data-ttu-id="4d152-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4d152-109">Member</span></span>|<span data-ttu-id="4d152-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4d152-110">Value</span></span>|<span data-ttu-id="4d152-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4d152-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d152-112">Нет</span><span class="sxs-lookup"><span data-stu-id="4d152-112">none</span></span>|<span data-ttu-id="4d152-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4d152-113">0</span></span>|<span data-ttu-id="4d152-114">Отправка ответов LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="4d152-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="4d152-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="4d152-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="4d152-116">1,1</span><span class="sxs-lookup"><span data-stu-id="4d152-116">1</span></span>|<span data-ttu-id="4d152-117">Отправлять LM & NTLM — использовать сеансовую безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="4d152-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="4d152-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="4d152-118">require128BitEncryption</span></span>|<span data-ttu-id="4d152-119">2</span><span class="sxs-lookup"><span data-stu-id="4d152-119">2</span></span>|<span data-ttu-id="4d152-120">Отправлять только LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="4d152-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="4d152-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="4d152-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="4d152-122">4</span><span class="sxs-lookup"><span data-stu-id="4d152-122">3</span></span>|<span data-ttu-id="4d152-123">Отправлять только LM & только ответы NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="4d152-123">Send LM & NTLMv2 responses only</span></span>|



