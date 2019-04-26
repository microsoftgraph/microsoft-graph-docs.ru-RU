---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88872e6d37afd1820559018bff6943e3ee623a0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563534"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="8f314-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="8f314-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="8f314-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f314-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f314-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f314-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f314-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="8f314-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="8f314-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8f314-107">Members</span></span>
|<span data-ttu-id="8f314-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8f314-108">Member</span></span>|<span data-ttu-id="8f314-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8f314-109">Value</span></span>|<span data-ttu-id="8f314-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8f314-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f314-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8f314-111">notConfigured</span></span>|<span data-ttu-id="8f314-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8f314-112">0</span></span>|<span data-ttu-id="8f314-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антиВирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="8f314-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="8f314-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="8f314-114">high</span></span>|<span data-ttu-id="8f314-115">1 </span><span class="sxs-lookup"><span data-stu-id="8f314-115">1</span></span>|<span data-ttu-id="8f314-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="8f314-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="8f314-117">Хигхплус</span><span class="sxs-lookup"><span data-stu-id="8f314-117">highPlus</span></span>|<span data-ttu-id="8f314-118">2 </span><span class="sxs-lookup"><span data-stu-id="8f314-118">2</span></span>|<span data-ttu-id="8f314-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="8f314-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="8f314-120">Зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="8f314-120">zeroTolerance</span></span>|<span data-ttu-id="8f314-121">3 </span><span class="sxs-lookup"><span data-stu-id="8f314-121">3</span></span>|<span data-ttu-id="8f314-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="8f314-122">Zero tolerance blocks all unknown executables</span></span>|





