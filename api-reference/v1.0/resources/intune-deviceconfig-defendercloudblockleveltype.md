---
title: Тип перечисления defenderCloudBlockLevelType
description: Возможные значения уровня блока облако
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e27ec7042522d7d4c83463b062cdc0c4c109daeb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951413"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="143e6-103">Тип перечисления defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="143e6-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="143e6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="143e6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="143e6-105">Возможные значения уровня блока облако</span><span class="sxs-lookup"><span data-stu-id="143e6-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="143e6-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="143e6-106">Members</span></span>
|<span data-ttu-id="143e6-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="143e6-107">Member</span></span>|<span data-ttu-id="143e6-108">Значение</span><span class="sxs-lookup"><span data-stu-id="143e6-108">Value</span></span>|<span data-ttu-id="143e6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="143e6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="143e6-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="143e6-110">notConfigured</span></span>|<span data-ttu-id="143e6-111">0</span><span class="sxs-lookup"><span data-stu-id="143e6-111">0</span></span>|<span data-ttu-id="143e6-112">Значение по умолчанию использует блокировки антивирусной программы Защитник Windows по умолчанию на уровне и обеспечивает строгое обнаружение без увеличения риска для обнаружения допустимые файлов</span><span class="sxs-lookup"><span data-stu-id="143e6-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="143e6-113">Высокая</span><span class="sxs-lookup"><span data-stu-id="143e6-113">high</span></span>|<span data-ttu-id="143e6-114">1</span><span class="sxs-lookup"><span data-stu-id="143e6-114">1</span></span>|<span data-ttu-id="143e6-115">High применяется повышенный уровень обнаружения.</span><span class="sxs-lookup"><span data-stu-id="143e6-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="143e6-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="143e6-116">highPlus</span></span>|<span data-ttu-id="143e6-117">2</span><span class="sxs-lookup"><span data-stu-id="143e6-117">2</span></span>|<span data-ttu-id="143e6-118">Высокая + использует высокий уровень и предоставляет средства защиты сложения</span><span class="sxs-lookup"><span data-stu-id="143e6-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="143e6-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="143e6-119">zeroTolerance</span></span>|<span data-ttu-id="143e6-120">3</span><span class="sxs-lookup"><span data-stu-id="143e6-120">3</span></span>|<span data-ttu-id="143e6-121">Ноль отказоустойчивости блокирует все неизвестные исполняемых файлов</span><span class="sxs-lookup"><span data-stu-id="143e6-121">Zero tolerance blocks all unknown executables</span></span>|



