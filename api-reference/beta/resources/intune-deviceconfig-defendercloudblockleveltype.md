---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f798e4b7572cc2593d0d742ecbdebf81d65507d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979867"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="4fab5-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="4fab5-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="4fab5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fab5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fab5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fab5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fab5-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="4fab5-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="4fab5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4fab5-107">Members</span></span>
|<span data-ttu-id="4fab5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4fab5-108">Member</span></span>|<span data-ttu-id="4fab5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4fab5-109">Value</span></span>|<span data-ttu-id="4fab5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4fab5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fab5-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4fab5-111">notConfigured</span></span>|<span data-ttu-id="4fab5-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4fab5-112">0</span></span>|<span data-ttu-id="4fab5-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="4fab5-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="4fab5-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="4fab5-114">high</span></span>|<span data-ttu-id="4fab5-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4fab5-115">1</span></span>|<span data-ttu-id="4fab5-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="4fab5-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="4fab5-117">Хигхплус</span><span class="sxs-lookup"><span data-stu-id="4fab5-117">highPlus</span></span>|<span data-ttu-id="4fab5-118">2</span><span class="sxs-lookup"><span data-stu-id="4fab5-118">2</span></span>|<span data-ttu-id="4fab5-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="4fab5-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="4fab5-120">Зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="4fab5-120">zeroTolerance</span></span>|<span data-ttu-id="4fab5-121">4</span><span class="sxs-lookup"><span data-stu-id="4fab5-121">3</span></span>|<span data-ttu-id="4fab5-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="4fab5-122">Zero tolerance blocks all unknown executables</span></span>|





