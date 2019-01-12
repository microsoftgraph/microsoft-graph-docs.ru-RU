---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня блока облако
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 13f8828478eb063eaa25d8561d5a254c86f4b856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924722"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="0f915-103">Тип перечисления defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="0f915-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="0f915-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f915-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f915-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f915-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f915-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f915-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f915-107">Возможные значения уровня блока облако</span><span class="sxs-lookup"><span data-stu-id="0f915-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="0f915-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0f915-108">Members</span></span>
|<span data-ttu-id="0f915-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0f915-109">Member</span></span>|<span data-ttu-id="0f915-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0f915-110">Value</span></span>|<span data-ttu-id="0f915-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f915-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f915-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0f915-112">notConfigured</span></span>|<span data-ttu-id="0f915-113">0</span><span class="sxs-lookup"><span data-stu-id="0f915-113">0</span></span>|<span data-ttu-id="0f915-114">Значение по умолчанию использует блокировки антивирусной программы Защитник Windows по умолчанию на уровне и обеспечивает строгое обнаружение без увеличения риска для обнаружения допустимые файлов</span><span class="sxs-lookup"><span data-stu-id="0f915-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="0f915-115">Высокая</span><span class="sxs-lookup"><span data-stu-id="0f915-115">high</span></span>|<span data-ttu-id="0f915-116">1</span><span class="sxs-lookup"><span data-stu-id="0f915-116">1</span></span>|<span data-ttu-id="0f915-117">High применяется повышенный уровень обнаружения.</span><span class="sxs-lookup"><span data-stu-id="0f915-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="0f915-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="0f915-118">highPlus</span></span>|<span data-ttu-id="0f915-119">2</span><span class="sxs-lookup"><span data-stu-id="0f915-119">2</span></span>|<span data-ttu-id="0f915-120">Высокая + использует высокий уровень и предоставляет средства защиты сложения</span><span class="sxs-lookup"><span data-stu-id="0f915-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="0f915-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="0f915-121">zeroTolerance</span></span>|<span data-ttu-id="0f915-122">3</span><span class="sxs-lookup"><span data-stu-id="0f915-122">3</span></span>|<span data-ttu-id="0f915-123">Ноль отказоустойчивости блокирует все неизвестные исполняемых файлов</span><span class="sxs-lookup"><span data-stu-id="0f915-123">Zero tolerance blocks all unknown executables</span></span>|





