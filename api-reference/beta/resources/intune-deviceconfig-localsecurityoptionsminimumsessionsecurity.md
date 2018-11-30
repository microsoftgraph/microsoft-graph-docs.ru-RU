---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
ms.openlocfilehash: 969c7d6576c613f5214bfc3b8a5a1ad36722f0df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080666"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="32812-103">Тип перечисления localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="32812-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="32812-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="32812-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32812-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32812-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32812-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="32812-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32812-107">Возможные значения для LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="32812-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="32812-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="32812-108">Members</span></span>
|<span data-ttu-id="32812-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="32812-109">Member</span></span>|<span data-ttu-id="32812-110">Значение</span><span class="sxs-lookup"><span data-stu-id="32812-110">Value</span></span>|<span data-ttu-id="32812-111">Description</span><span class="sxs-lookup"><span data-stu-id="32812-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32812-112">Нет</span><span class="sxs-lookup"><span data-stu-id="32812-112">none</span></span>|<span data-ttu-id="32812-113">0</span><span class="sxs-lookup"><span data-stu-id="32812-113">0</span></span>|<span data-ttu-id="32812-114">Отправлять ответы LM и NTLM</span><span class="sxs-lookup"><span data-stu-id="32812-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="32812-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="32812-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="32812-116">1</span><span class="sxs-lookup"><span data-stu-id="32812-116">1</span></span>|<span data-ttu-id="32812-117">Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование</span><span class="sxs-lookup"><span data-stu-id="32812-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="32812-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="32812-118">require128BitEncryption</span></span>|<span data-ttu-id="32812-119">2</span><span class="sxs-lookup"><span data-stu-id="32812-119">2</span></span>|<span data-ttu-id="32812-120">Отправлять LM и NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="32812-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="32812-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="32812-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="32812-122">3</span><span class="sxs-lookup"><span data-stu-id="32812-122">3</span></span>|<span data-ttu-id="32812-123">Отправлять LM и NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="32812-123">Send LM & NTLMv2 responses only</span></span>|





