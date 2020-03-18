---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3afc9a0bdf5d25c4496cb2dcf4a7ef013ac0785d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795625"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="7bb4c-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="7bb4c-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="7bb4c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bb4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bb4c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bb4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bb4c-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="7bb4c-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="7bb4c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7bb4c-107">Members</span></span>
|<span data-ttu-id="7bb4c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7bb4c-108">Member</span></span>|<span data-ttu-id="7bb4c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7bb4c-109">Value</span></span>|<span data-ttu-id="7bb4c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7bb4c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bb4c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7bb4c-111">notConfigured</span></span>|<span data-ttu-id="7bb4c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7bb4c-112">0</span></span>|<span data-ttu-id="7bb4c-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="7bb4c-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="7bb4c-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="7bb4c-114">high</span></span>|<span data-ttu-id="7bb4c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="7bb4c-115">1</span></span>|<span data-ttu-id="7bb4c-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="7bb4c-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="7bb4c-117">хигхплус</span><span class="sxs-lookup"><span data-stu-id="7bb4c-117">highPlus</span></span>|<span data-ttu-id="7bb4c-118">2</span><span class="sxs-lookup"><span data-stu-id="7bb4c-118">2</span></span>|<span data-ttu-id="7bb4c-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="7bb4c-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="7bb4c-120">зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="7bb4c-120">zeroTolerance</span></span>|<span data-ttu-id="7bb4c-121">4</span><span class="sxs-lookup"><span data-stu-id="7bb4c-121">3</span></span>|<span data-ttu-id="7bb4c-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="7bb4c-122">Zero tolerance blocks all unknown executables</span></span>|



