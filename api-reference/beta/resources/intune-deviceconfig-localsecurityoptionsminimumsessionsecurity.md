---
title: Тип перечисления localSecurityOptionsMinimumSessionSecurity
description: Возможные значения для LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
ms.openlocfilehash: 5feabd9c84ec42f55bb45b952be5af834fd84498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350639"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="6e752-103">Тип перечисления localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6e752-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="6e752-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e752-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e752-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e752-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e752-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6e752-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e752-107">Возможные значения для LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6e752-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="6e752-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6e752-108">Members</span></span>
|<span data-ttu-id="6e752-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6e752-109">Member</span></span>|<span data-ttu-id="6e752-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6e752-110">Value</span></span>|<span data-ttu-id="6e752-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6e752-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e752-112">none</span><span class="sxs-lookup"><span data-stu-id="6e752-112">none</span></span>|<span data-ttu-id="6e752-113">0</span><span class="sxs-lookup"><span data-stu-id="6e752-113">0</span></span>|<span data-ttu-id="6e752-114">Отправлять ответы LM и NTLM</span><span class="sxs-lookup"><span data-stu-id="6e752-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="6e752-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6e752-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="6e752-116">1</span><span class="sxs-lookup"><span data-stu-id="6e752-116">1</span></span>|<span data-ttu-id="6e752-117">Отправлять LM и NTLM использования NTLMv2 сеансовая безопасность, если согласование</span><span class="sxs-lookup"><span data-stu-id="6e752-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="6e752-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="6e752-118">require128BitEncryption</span></span>|<span data-ttu-id="6e752-119">2</span><span class="sxs-lookup"><span data-stu-id="6e752-119">2</span></span>|<span data-ttu-id="6e752-120">Отправлять LM и NTLM ответы</span><span class="sxs-lookup"><span data-stu-id="6e752-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="6e752-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="6e752-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="6e752-122">3</span><span class="sxs-lookup"><span data-stu-id="6e752-122">3</span></span>|<span data-ttu-id="6e752-123">Отправлять LM и NTLMv2 ответы</span><span class="sxs-lookup"><span data-stu-id="6e752-123">Send LM & NTLMv2 responses only</span></span>|





