---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 822c996d788fd5edb5c92f876c725b771b051c15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952484"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="8cb53-103">Тип перечисления localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8cb53-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="8cb53-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cb53-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cb53-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cb53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cb53-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8cb53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cb53-107">Возможные значения для LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8cb53-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="8cb53-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8cb53-108">Members</span></span>
|<span data-ttu-id="8cb53-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8cb53-109">Member</span></span>|<span data-ttu-id="8cb53-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8cb53-110">Value</span></span>|<span data-ttu-id="8cb53-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8cb53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb53-112">Нет</span><span class="sxs-lookup"><span data-stu-id="8cb53-112">none</span></span>|<span data-ttu-id="8cb53-113">0</span><span class="sxs-lookup"><span data-stu-id="8cb53-113">0</span></span>|<span data-ttu-id="8cb53-114">Отправлять ответы LM и NTLM</span><span class="sxs-lookup"><span data-stu-id="8cb53-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="8cb53-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="8cb53-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="8cb53-116">1</span><span class="sxs-lookup"><span data-stu-id="8cb53-116">1</span></span>|<span data-ttu-id="8cb53-117">Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование</span><span class="sxs-lookup"><span data-stu-id="8cb53-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="8cb53-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="8cb53-118">require128BitEncryption</span></span>|<span data-ttu-id="8cb53-119">2</span><span class="sxs-lookup"><span data-stu-id="8cb53-119">2</span></span>|<span data-ttu-id="8cb53-120">Отправлять LM и NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="8cb53-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="8cb53-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="8cb53-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="8cb53-122">3</span><span class="sxs-lookup"><span data-stu-id="8cb53-122">3</span></span>|<span data-ttu-id="8cb53-123">Отправлять LM и NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="8cb53-123">Send LM & NTLMv2 responses only</span></span>|





