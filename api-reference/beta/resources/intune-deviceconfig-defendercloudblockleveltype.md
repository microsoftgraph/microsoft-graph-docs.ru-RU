---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня блока облако
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b309184623cff19e44ee5afea311d46fa89210fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425913"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="46801-103">Тип перечисления defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="46801-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="46801-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46801-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46801-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46801-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46801-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46801-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46801-107">Возможные значения уровня блока облако</span><span class="sxs-lookup"><span data-stu-id="46801-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="46801-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="46801-108">Members</span></span>
|<span data-ttu-id="46801-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="46801-109">Member</span></span>|<span data-ttu-id="46801-110">Значение</span><span class="sxs-lookup"><span data-stu-id="46801-110">Value</span></span>|<span data-ttu-id="46801-111">Описание</span><span class="sxs-lookup"><span data-stu-id="46801-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46801-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="46801-112">notConfigured</span></span>|<span data-ttu-id="46801-113">0</span><span class="sxs-lookup"><span data-stu-id="46801-113">0</span></span>|<span data-ttu-id="46801-114">Значение по умолчанию использует блокировки антивирусной программы Защитник Windows по умолчанию на уровне и обеспечивает строгое обнаружение без увеличения риска для обнаружения допустимые файлов</span><span class="sxs-lookup"><span data-stu-id="46801-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="46801-115">Высокая</span><span class="sxs-lookup"><span data-stu-id="46801-115">high</span></span>|<span data-ttu-id="46801-116">1</span><span class="sxs-lookup"><span data-stu-id="46801-116">1</span></span>|<span data-ttu-id="46801-117">High применяется повышенный уровень обнаружения.</span><span class="sxs-lookup"><span data-stu-id="46801-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="46801-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="46801-118">highPlus</span></span>|<span data-ttu-id="46801-119">2</span><span class="sxs-lookup"><span data-stu-id="46801-119">2</span></span>|<span data-ttu-id="46801-120">Высокая + использует высокий уровень и предоставляет средства защиты сложения</span><span class="sxs-lookup"><span data-stu-id="46801-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="46801-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="46801-121">zeroTolerance</span></span>|<span data-ttu-id="46801-122">3</span><span class="sxs-lookup"><span data-stu-id="46801-122">3</span></span>|<span data-ttu-id="46801-123">Ноль отказоустойчивости блокирует все неизвестные исполняемых файлов</span><span class="sxs-lookup"><span data-stu-id="46801-123">Zero tolerance blocks all unknown executables</span></span>|




