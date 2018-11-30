---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня блока облако
ms.openlocfilehash: 6ea336418a90a3d4caeab074cb71fce997ea1275
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026412"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="e7780-103">Тип перечисления defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="e7780-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="e7780-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7780-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7780-105">Возможные значения уровня блока облако</span><span class="sxs-lookup"><span data-stu-id="e7780-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="e7780-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="e7780-106">Members</span></span>
|<span data-ttu-id="e7780-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="e7780-107">Member</span></span>|<span data-ttu-id="e7780-108">Значение</span><span class="sxs-lookup"><span data-stu-id="e7780-108">Value</span></span>|<span data-ttu-id="e7780-109">Description</span><span class="sxs-lookup"><span data-stu-id="e7780-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7780-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e7780-110">notConfigured</span></span>|<span data-ttu-id="e7780-111">0</span><span class="sxs-lookup"><span data-stu-id="e7780-111">0</span></span>|<span data-ttu-id="e7780-112">Значение по умолчанию использует блокировки антивирусной программы Защитник Windows по умолчанию на уровне и обеспечивает строгое обнаружение без увеличения риска для обнаружения допустимые файлов</span><span class="sxs-lookup"><span data-stu-id="e7780-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="e7780-113">Высокая</span><span class="sxs-lookup"><span data-stu-id="e7780-113">high</span></span>|<span data-ttu-id="e7780-114">1</span><span class="sxs-lookup"><span data-stu-id="e7780-114">1</span></span>|<span data-ttu-id="e7780-115">High применяется повышенный уровень обнаружения.</span><span class="sxs-lookup"><span data-stu-id="e7780-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="e7780-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="e7780-116">highPlus</span></span>|<span data-ttu-id="e7780-117">2</span><span class="sxs-lookup"><span data-stu-id="e7780-117">2</span></span>|<span data-ttu-id="e7780-118">Высокая + использует высокий уровень и предоставляет средства защиты сложения</span><span class="sxs-lookup"><span data-stu-id="e7780-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="e7780-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="e7780-119">zeroTolerance</span></span>|<span data-ttu-id="e7780-120">3</span><span class="sxs-lookup"><span data-stu-id="e7780-120">3</span></span>|<span data-ttu-id="e7780-121">Ноль отказоустойчивости блокирует все неизвестные исполняемых файлов</span><span class="sxs-lookup"><span data-stu-id="e7780-121">Zero tolerance blocks all unknown executables</span></span>|



