---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 928a39e25a02286159ba886bed9c1415b038edbf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001791"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="04c3e-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="04c3e-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="04c3e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04c3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04c3e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04c3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04c3e-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="04c3e-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="04c3e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="04c3e-107">Members</span></span>
|<span data-ttu-id="04c3e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="04c3e-108">Member</span></span>|<span data-ttu-id="04c3e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="04c3e-109">Value</span></span>|<span data-ttu-id="04c3e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="04c3e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04c3e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="04c3e-111">notConfigured</span></span>|<span data-ttu-id="04c3e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="04c3e-112">0</span></span>|<span data-ttu-id="04c3e-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="04c3e-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="04c3e-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="04c3e-114">high</span></span>|<span data-ttu-id="04c3e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="04c3e-115">1</span></span>|<span data-ttu-id="04c3e-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="04c3e-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="04c3e-117">Хигхплус</span><span class="sxs-lookup"><span data-stu-id="04c3e-117">highPlus</span></span>|<span data-ttu-id="04c3e-118">2</span><span class="sxs-lookup"><span data-stu-id="04c3e-118">2</span></span>|<span data-ttu-id="04c3e-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="04c3e-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="04c3e-120">Зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="04c3e-120">zeroTolerance</span></span>|<span data-ttu-id="04c3e-121">4</span><span class="sxs-lookup"><span data-stu-id="04c3e-121">3</span></span>|<span data-ttu-id="04c3e-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="04c3e-122">Zero tolerance blocks all unknown executables</span></span>|





