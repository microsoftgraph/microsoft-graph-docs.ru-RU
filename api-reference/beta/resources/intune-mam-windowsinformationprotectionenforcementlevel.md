---
title: Тип перечисления windowsInformationProtectionEnforcementLevel
description: Возможные значения для защиты НЗП принудительное применение уровней
ms.openlocfilehash: a590132f80028af513d4244f49904267b3a85f50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079145"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="8dbb5-103">Тип перечисления windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="8dbb5-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="8dbb5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8dbb5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dbb5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dbb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8dbb5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8dbb5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8dbb5-107">Возможные значения для защиты НЗП принудительное применение уровней</span><span class="sxs-lookup"><span data-stu-id="8dbb5-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="8dbb5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8dbb5-108">Members</span></span>
|<span data-ttu-id="8dbb5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8dbb5-109">Member</span></span>|<span data-ttu-id="8dbb5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8dbb5-110">Value</span></span>|<span data-ttu-id="8dbb5-111">Description</span><span class="sxs-lookup"><span data-stu-id="8dbb5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dbb5-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="8dbb5-112">noProtection</span></span>|<span data-ttu-id="8dbb5-113">0</span><span class="sxs-lookup"><span data-stu-id="8dbb5-113">0</span></span>|<span data-ttu-id="8dbb5-114">Принудительное применение без защиты</span><span class="sxs-lookup"><span data-stu-id="8dbb5-114">No protection enforcement</span></span>|
|<span data-ttu-id="8dbb5-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="8dbb5-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="8dbb5-116">1</span><span class="sxs-lookup"><span data-stu-id="8dbb5-116">1</span></span>|<span data-ttu-id="8dbb5-117">Шифрование и только аудита</span><span class="sxs-lookup"><span data-stu-id="8dbb5-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="8dbb5-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="8dbb5-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="8dbb5-119">2</span><span class="sxs-lookup"><span data-stu-id="8dbb5-119">2</span></span>|<span data-ttu-id="8dbb5-120">Шифрование, аудита и запрашивать пользователя</span><span class="sxs-lookup"><span data-stu-id="8dbb5-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="8dbb5-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="8dbb5-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="8dbb5-122">3</span><span class="sxs-lookup"><span data-stu-id="8dbb5-122">3</span></span>|<span data-ttu-id="8dbb5-123">Шифрование, аудита и блокировки</span><span class="sxs-lookup"><span data-stu-id="8dbb5-123">Encrypt, Audit and Block</span></span>|





