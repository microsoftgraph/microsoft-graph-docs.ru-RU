---
title: Тип перечисления eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954458"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="dc8c7-103">Тип перечисления eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc8c7-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="dc8c7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc8c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc8c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc8c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc8c7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc8c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc8c7-107">Доступные параметры для конфигурации EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="dc8c7-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="dc8c7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dc8c7-108">Members</span></span>
|<span data-ttu-id="dc8c7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dc8c7-109">Member</span></span>|<span data-ttu-id="dc8c7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dc8c7-110">Value</span></span>|<span data-ttu-id="dc8c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc8c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc8c7-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="dc8c7-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="dc8c7-113">0</span><span class="sxs-lookup"><span data-stu-id="dc8c7-113">0</span></span>|<span data-ttu-id="dc8c7-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="dc8c7-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="dc8c7-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="dc8c7-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="dc8c7-116">1</span><span class="sxs-lookup"><span data-stu-id="dc8c7-116">1</span></span>|<span data-ttu-id="dc8c7-117">Использование защиты безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="dc8c7-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="dc8c7-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="dc8c7-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="dc8c7-119">2</span><span class="sxs-lookup"><span data-stu-id="dc8c7-119">2</span></span>|<span data-ttu-id="dc8c7-120">Использование защищенного доступа учетные данные (PAC) и подготовки идентификационные</span><span class="sxs-lookup"><span data-stu-id="dc8c7-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="dc8c7-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="dc8c7-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="dc8c7-122">3</span><span class="sxs-lookup"><span data-stu-id="dc8c7-122">3</span></span>|<span data-ttu-id="dc8c7-123">Использование защищенного доступа учетные данные (PAC), PAC подготовки и делать это анонимного доступа.</span><span class="sxs-lookup"><span data-stu-id="dc8c7-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





