---
title: Тип перечисления windowsInformationProtectionEnforcementLevel
description: Возможные значения для защиты НЗП принудительное применение уровней
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4661c80655defe85f27ac8259a961955552f7021
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964174"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="4b0c0-103">Тип перечисления windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="4b0c0-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="4b0c0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b0c0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b0c0-105">Возможные значения для защиты НЗП принудительное применение уровней</span><span class="sxs-lookup"><span data-stu-id="4b0c0-105">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="4b0c0-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="4b0c0-106">Members</span></span>
|<span data-ttu-id="4b0c0-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="4b0c0-107">Member</span></span>|<span data-ttu-id="4b0c0-108">Значение</span><span class="sxs-lookup"><span data-stu-id="4b0c0-108">Value</span></span>|<span data-ttu-id="4b0c0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4b0c0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b0c0-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="4b0c0-110">noProtection</span></span>|<span data-ttu-id="4b0c0-111">0</span><span class="sxs-lookup"><span data-stu-id="4b0c0-111">0</span></span>|<span data-ttu-id="4b0c0-112">Принудительное применение без защиты</span><span class="sxs-lookup"><span data-stu-id="4b0c0-112">No protection enforcement</span></span>|
|<span data-ttu-id="4b0c0-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="4b0c0-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="4b0c0-114">1</span><span class="sxs-lookup"><span data-stu-id="4b0c0-114">1</span></span>|<span data-ttu-id="4b0c0-115">Шифрование и только аудита</span><span class="sxs-lookup"><span data-stu-id="4b0c0-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="4b0c0-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="4b0c0-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="4b0c0-117">2</span><span class="sxs-lookup"><span data-stu-id="4b0c0-117">2</span></span>|<span data-ttu-id="4b0c0-118">Шифрование, аудита и запрашивать пользователя</span><span class="sxs-lookup"><span data-stu-id="4b0c0-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="4b0c0-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="4b0c0-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="4b0c0-120">3</span><span class="sxs-lookup"><span data-stu-id="4b0c0-120">3</span></span>|<span data-ttu-id="4b0c0-121">Шифрование, аудита и блокировки</span><span class="sxs-lookup"><span data-stu-id="4b0c0-121">Encrypt, Audit and Block</span></span>|



