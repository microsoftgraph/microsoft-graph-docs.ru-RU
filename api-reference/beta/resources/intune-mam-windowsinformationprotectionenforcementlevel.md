---
title: Тип перечисления windowsInformationProtectionEnforcementLevel
description: Возможные значения для защиты НЗП принудительное применение уровней
author: tfitzmac
ms.openlocfilehash: cb30ffb58b129fc302d7896c148072a54b98c0a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315164"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="d6418-103">Тип перечисления windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d6418-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="d6418-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6418-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6418-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6418-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6418-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6418-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6418-107">Возможные значения для защиты НЗП принудительное применение уровней</span><span class="sxs-lookup"><span data-stu-id="d6418-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="d6418-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d6418-108">Members</span></span>
|<span data-ttu-id="d6418-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d6418-109">Member</span></span>|<span data-ttu-id="d6418-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d6418-110">Value</span></span>|<span data-ttu-id="d6418-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d6418-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6418-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="d6418-112">noProtection</span></span>|<span data-ttu-id="d6418-113">0</span><span class="sxs-lookup"><span data-stu-id="d6418-113">0</span></span>|<span data-ttu-id="d6418-114">Принудительное применение без защиты</span><span class="sxs-lookup"><span data-stu-id="d6418-114">No protection enforcement</span></span>|
|<span data-ttu-id="d6418-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="d6418-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="d6418-116">1</span><span class="sxs-lookup"><span data-stu-id="d6418-116">1</span></span>|<span data-ttu-id="d6418-117">Шифрование и только аудита</span><span class="sxs-lookup"><span data-stu-id="d6418-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="d6418-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="d6418-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="d6418-119">2</span><span class="sxs-lookup"><span data-stu-id="d6418-119">2</span></span>|<span data-ttu-id="d6418-120">Шифрование, аудита и запрашивать пользователя</span><span class="sxs-lookup"><span data-stu-id="d6418-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="d6418-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="d6418-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="d6418-122">3</span><span class="sxs-lookup"><span data-stu-id="d6418-122">3</span></span>|<span data-ttu-id="d6418-123">Шифрование, аудита и блокировки</span><span class="sxs-lookup"><span data-stu-id="d6418-123">Encrypt, Audit and Block</span></span>|





