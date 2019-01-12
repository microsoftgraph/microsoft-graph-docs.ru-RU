---
title: Тип перечисления windowsInformationProtectionEnforcementLevel
description: Возможные значения для защиты НЗП принудительное применение уровней
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed087465d05ba91bcdc1f8cff7fec0aba567420a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913410"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="b22a9-103">Тип перечисления windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="b22a9-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="b22a9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b22a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b22a9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b22a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b22a9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b22a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b22a9-107">Возможные значения для защиты НЗП принудительное применение уровней</span><span class="sxs-lookup"><span data-stu-id="b22a9-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="b22a9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b22a9-108">Members</span></span>
|<span data-ttu-id="b22a9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b22a9-109">Member</span></span>|<span data-ttu-id="b22a9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b22a9-110">Value</span></span>|<span data-ttu-id="b22a9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b22a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b22a9-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="b22a9-112">noProtection</span></span>|<span data-ttu-id="b22a9-113">0</span><span class="sxs-lookup"><span data-stu-id="b22a9-113">0</span></span>|<span data-ttu-id="b22a9-114">Принудительное применение без защиты</span><span class="sxs-lookup"><span data-stu-id="b22a9-114">No protection enforcement</span></span>|
|<span data-ttu-id="b22a9-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="b22a9-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="b22a9-116">1</span><span class="sxs-lookup"><span data-stu-id="b22a9-116">1</span></span>|<span data-ttu-id="b22a9-117">Шифрование и только аудита</span><span class="sxs-lookup"><span data-stu-id="b22a9-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="b22a9-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="b22a9-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="b22a9-119">2</span><span class="sxs-lookup"><span data-stu-id="b22a9-119">2</span></span>|<span data-ttu-id="b22a9-120">Шифрование, аудита и запрашивать пользователя</span><span class="sxs-lookup"><span data-stu-id="b22a9-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="b22a9-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="b22a9-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="b22a9-122">3</span><span class="sxs-lookup"><span data-stu-id="b22a9-122">3</span></span>|<span data-ttu-id="b22a9-123">Шифрование, аудита и блокировки</span><span class="sxs-lookup"><span data-stu-id="b22a9-123">Encrypt, Audit and Block</span></span>|





