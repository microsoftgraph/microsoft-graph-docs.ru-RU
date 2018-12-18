---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня блока облако
author: tfitzmac
ms.openlocfilehash: c58c844097c18ff86beaef4a0e48d9b8a39043f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317446"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="532a3-103">Тип перечисления defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="532a3-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="532a3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="532a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="532a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="532a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="532a3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="532a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="532a3-107">Возможные значения уровня блока облако</span><span class="sxs-lookup"><span data-stu-id="532a3-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="532a3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="532a3-108">Members</span></span>
|<span data-ttu-id="532a3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="532a3-109">Member</span></span>|<span data-ttu-id="532a3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="532a3-110">Value</span></span>|<span data-ttu-id="532a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="532a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="532a3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="532a3-112">notConfigured</span></span>|<span data-ttu-id="532a3-113">0</span><span class="sxs-lookup"><span data-stu-id="532a3-113">0</span></span>|<span data-ttu-id="532a3-114">Значение по умолчанию использует блокировки антивирусной программы Защитник Windows по умолчанию на уровне и обеспечивает строгое обнаружение без увеличения риска для обнаружения допустимые файлов</span><span class="sxs-lookup"><span data-stu-id="532a3-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="532a3-115">Высокая</span><span class="sxs-lookup"><span data-stu-id="532a3-115">high</span></span>|<span data-ttu-id="532a3-116">1</span><span class="sxs-lookup"><span data-stu-id="532a3-116">1</span></span>|<span data-ttu-id="532a3-117">High применяется повышенный уровень обнаружения.</span><span class="sxs-lookup"><span data-stu-id="532a3-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="532a3-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="532a3-118">highPlus</span></span>|<span data-ttu-id="532a3-119">2</span><span class="sxs-lookup"><span data-stu-id="532a3-119">2</span></span>|<span data-ttu-id="532a3-120">Высокая + использует высокий уровень и предоставляет средства защиты сложения</span><span class="sxs-lookup"><span data-stu-id="532a3-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="532a3-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="532a3-121">zeroTolerance</span></span>|<span data-ttu-id="532a3-122">3</span><span class="sxs-lookup"><span data-stu-id="532a3-122">3</span></span>|<span data-ttu-id="532a3-123">Ноль отказоустойчивости блокирует все неизвестные исполняемых файлов</span><span class="sxs-lookup"><span data-stu-id="532a3-123">Zero tolerance blocks all unknown executables</span></span>|





