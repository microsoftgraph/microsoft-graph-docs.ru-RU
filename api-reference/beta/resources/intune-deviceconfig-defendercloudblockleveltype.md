---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbf442a11335602c510a210d7bd805b2a76eb7df
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156926"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="bdf97-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="bdf97-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="bdf97-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdf97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdf97-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdf97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdf97-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="bdf97-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="bdf97-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bdf97-107">Members</span></span>
|<span data-ttu-id="bdf97-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bdf97-108">Member</span></span>|<span data-ttu-id="bdf97-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bdf97-109">Value</span></span>|<span data-ttu-id="bdf97-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf97-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf97-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bdf97-111">notConfigured</span></span>|<span data-ttu-id="bdf97-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bdf97-112">0</span></span>|<span data-ttu-id="bdf97-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антиВирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="bdf97-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="bdf97-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="bdf97-114">high</span></span>|<span data-ttu-id="bdf97-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bdf97-115">1</span></span>|<span data-ttu-id="bdf97-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="bdf97-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="bdf97-117">Хигхплус</span><span class="sxs-lookup"><span data-stu-id="bdf97-117">highPlus</span></span>|<span data-ttu-id="bdf97-118">2</span><span class="sxs-lookup"><span data-stu-id="bdf97-118">2</span></span>|<span data-ttu-id="bdf97-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="bdf97-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="bdf97-120">Зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="bdf97-120">zeroTolerance</span></span>|<span data-ttu-id="bdf97-121">4</span><span class="sxs-lookup"><span data-stu-id="bdf97-121">3</span></span>|<span data-ttu-id="bdf97-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="bdf97-122">Zero tolerance blocks all unknown executables</span></span>|




