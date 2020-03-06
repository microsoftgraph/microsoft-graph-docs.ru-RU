---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd121a61106ae029ccacf2e393bd28ef34415045
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530895"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="f11c0-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="f11c0-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="f11c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f11c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f11c0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f11c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f11c0-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="f11c0-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="f11c0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f11c0-107">Members</span></span>
|<span data-ttu-id="f11c0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f11c0-108">Member</span></span>|<span data-ttu-id="f11c0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f11c0-109">Value</span></span>|<span data-ttu-id="f11c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f11c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f11c0-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f11c0-111">notConfigured</span></span>|<span data-ttu-id="f11c0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f11c0-112">0</span></span>|<span data-ttu-id="f11c0-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="f11c0-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="f11c0-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="f11c0-114">high</span></span>|<span data-ttu-id="f11c0-115">1 </span><span class="sxs-lookup"><span data-stu-id="f11c0-115">1</span></span>|<span data-ttu-id="f11c0-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="f11c0-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="f11c0-117">хигхплус</span><span class="sxs-lookup"><span data-stu-id="f11c0-117">highPlus</span></span>|<span data-ttu-id="f11c0-118">2 </span><span class="sxs-lookup"><span data-stu-id="f11c0-118">2</span></span>|<span data-ttu-id="f11c0-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="f11c0-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="f11c0-120">зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="f11c0-120">zeroTolerance</span></span>|<span data-ttu-id="f11c0-121">3 </span><span class="sxs-lookup"><span data-stu-id="f11c0-121">3</span></span>|<span data-ttu-id="f11c0-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="f11c0-122">Zero tolerance blocks all unknown executables</span></span>|




