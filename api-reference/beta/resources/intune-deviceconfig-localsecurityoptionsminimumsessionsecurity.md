---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396086"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="f56d9-103">Тип перечисления localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f56d9-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="f56d9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f56d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f56d9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f56d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f56d9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f56d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f56d9-107">Возможные значения для LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f56d9-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="f56d9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f56d9-108">Members</span></span>
|<span data-ttu-id="f56d9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f56d9-109">Member</span></span>|<span data-ttu-id="f56d9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f56d9-110">Value</span></span>|<span data-ttu-id="f56d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f56d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f56d9-112">none</span><span class="sxs-lookup"><span data-stu-id="f56d9-112">none</span></span>|<span data-ttu-id="f56d9-113">0</span><span class="sxs-lookup"><span data-stu-id="f56d9-113">0</span></span>|<span data-ttu-id="f56d9-114">Отправить LM & NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="f56d9-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="f56d9-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f56d9-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="f56d9-116">1</span><span class="sxs-lookup"><span data-stu-id="f56d9-116">1</span></span>|<span data-ttu-id="f56d9-117">Отправлять LM & использование NTLM сеансовая безопасность NTLMv2 при согласовании</span><span class="sxs-lookup"><span data-stu-id="f56d9-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="f56d9-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="f56d9-118">require128BitEncryption</span></span>|<span data-ttu-id="f56d9-119">2</span><span class="sxs-lookup"><span data-stu-id="f56d9-119">2</span></span>|<span data-ttu-id="f56d9-120">Отправлять LM & только NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="f56d9-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="f56d9-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="f56d9-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="f56d9-122">3</span><span class="sxs-lookup"><span data-stu-id="f56d9-122">3</span></span>|<span data-ttu-id="f56d9-123">Отправлять LM & только ответы NTLMv2</span><span class="sxs-lookup"><span data-stu-id="f56d9-123">Send LM & NTLMv2 responses only</span></span>|




