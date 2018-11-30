---
title: Тип перечисления eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
ms.openlocfilehash: b1771668ea627d2e873d54334e388989652736d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077235"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="58834-103">Тип перечисления eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="58834-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="58834-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58834-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58834-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58834-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58834-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58834-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58834-107">Доступные параметры для конфигурации EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="58834-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="58834-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="58834-108">Members</span></span>
|<span data-ttu-id="58834-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="58834-109">Member</span></span>|<span data-ttu-id="58834-110">Значение</span><span class="sxs-lookup"><span data-stu-id="58834-110">Value</span></span>|<span data-ttu-id="58834-111">Description</span><span class="sxs-lookup"><span data-stu-id="58834-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58834-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="58834-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="58834-113">0</span><span class="sxs-lookup"><span data-stu-id="58834-113">0</span></span>|<span data-ttu-id="58834-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="58834-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="58834-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="58834-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="58834-116">1</span><span class="sxs-lookup"><span data-stu-id="58834-116">1</span></span>|<span data-ttu-id="58834-117">Использование защиты безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="58834-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="58834-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="58834-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="58834-119">2</span><span class="sxs-lookup"><span data-stu-id="58834-119">2</span></span>|<span data-ttu-id="58834-120">Использование защищенного доступа учетные данные (PAC) и подготовки идентификационные</span><span class="sxs-lookup"><span data-stu-id="58834-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="58834-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="58834-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="58834-122">3</span><span class="sxs-lookup"><span data-stu-id="58834-122">3</span></span>|<span data-ttu-id="58834-123">Использование защищенного доступа учетные данные (PAC), PAC подготовки и делать это анонимного доступа.</span><span class="sxs-lookup"><span data-stu-id="58834-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





