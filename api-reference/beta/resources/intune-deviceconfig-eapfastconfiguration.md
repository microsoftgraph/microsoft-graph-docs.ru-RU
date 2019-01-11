---
title: Тип перечисления eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 499d6595980bcb6bca1ea93687399e8988a3bed7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811090"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="1c122-103">Тип перечисления eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c122-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="1c122-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1c122-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c122-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c122-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c122-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1c122-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c122-107">Доступные параметры для конфигурации EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="1c122-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="1c122-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1c122-108">Members</span></span>
|<span data-ttu-id="1c122-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1c122-109">Member</span></span>|<span data-ttu-id="1c122-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1c122-110">Value</span></span>|<span data-ttu-id="1c122-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1c122-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c122-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="1c122-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="1c122-113">0</span><span class="sxs-lookup"><span data-stu-id="1c122-113">0</span></span>|<span data-ttu-id="1c122-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="1c122-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="1c122-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="1c122-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="1c122-116">1</span><span class="sxs-lookup"><span data-stu-id="1c122-116">1</span></span>|<span data-ttu-id="1c122-117">Использование защиты безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="1c122-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="1c122-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="1c122-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="1c122-119">2</span><span class="sxs-lookup"><span data-stu-id="1c122-119">2</span></span>|<span data-ttu-id="1c122-120">Использование защищенного доступа учетные данные (PAC) и подготовки идентификационные</span><span class="sxs-lookup"><span data-stu-id="1c122-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="1c122-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="1c122-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="1c122-122">3</span><span class="sxs-lookup"><span data-stu-id="1c122-122">3</span></span>|<span data-ttu-id="1c122-123">Использование защищенного доступа учетные данные (PAC), PAC подготовки и делать это анонимного доступа.</span><span class="sxs-lookup"><span data-stu-id="1c122-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





