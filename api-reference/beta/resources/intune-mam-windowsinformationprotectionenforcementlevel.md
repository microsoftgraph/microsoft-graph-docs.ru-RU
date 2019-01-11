---
title: Тип перечисления windowsInformationProtectionEnforcementLevel
description: Возможные значения для защиты НЗП принудительное применение уровней
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5097682172281ece366a8f0389c314e2fb630190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868371"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="14201-103">Тип перечисления windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="14201-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="14201-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14201-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14201-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14201-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14201-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="14201-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14201-107">Возможные значения для защиты НЗП принудительное применение уровней</span><span class="sxs-lookup"><span data-stu-id="14201-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="14201-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="14201-108">Members</span></span>
|<span data-ttu-id="14201-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="14201-109">Member</span></span>|<span data-ttu-id="14201-110">Значение</span><span class="sxs-lookup"><span data-stu-id="14201-110">Value</span></span>|<span data-ttu-id="14201-111">Описание</span><span class="sxs-lookup"><span data-stu-id="14201-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14201-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="14201-112">noProtection</span></span>|<span data-ttu-id="14201-113">0</span><span class="sxs-lookup"><span data-stu-id="14201-113">0</span></span>|<span data-ttu-id="14201-114">Принудительное применение без защиты</span><span class="sxs-lookup"><span data-stu-id="14201-114">No protection enforcement</span></span>|
|<span data-ttu-id="14201-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="14201-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="14201-116">1</span><span class="sxs-lookup"><span data-stu-id="14201-116">1</span></span>|<span data-ttu-id="14201-117">Шифрование и только аудита</span><span class="sxs-lookup"><span data-stu-id="14201-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="14201-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="14201-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="14201-119">2</span><span class="sxs-lookup"><span data-stu-id="14201-119">2</span></span>|<span data-ttu-id="14201-120">Шифрование, аудита и запрашивать пользователя</span><span class="sxs-lookup"><span data-stu-id="14201-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="14201-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="14201-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="14201-122">3</span><span class="sxs-lookup"><span data-stu-id="14201-122">3</span></span>|<span data-ttu-id="14201-123">Шифрование, аудита и блокировки</span><span class="sxs-lookup"><span data-stu-id="14201-123">Encrypt, Audit and Block</span></span>|





