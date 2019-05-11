---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c83618e3c730140e4e667810fe7e91e1fb6bed7f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947374"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="0dda8-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="0dda8-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="0dda8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dda8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dda8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0dda8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dda8-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="0dda8-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="0dda8-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0dda8-107">Members</span></span>
|<span data-ttu-id="0dda8-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0dda8-108">Member</span></span>|<span data-ttu-id="0dda8-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0dda8-109">Value</span></span>|<span data-ttu-id="0dda8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0dda8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dda8-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0dda8-111">notConfigured</span></span>|<span data-ttu-id="0dda8-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0dda8-112">0</span></span>|<span data-ttu-id="0dda8-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="0dda8-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="0dda8-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="0dda8-114">high</span></span>|<span data-ttu-id="0dda8-115">1,1</span><span class="sxs-lookup"><span data-stu-id="0dda8-115">1</span></span>|<span data-ttu-id="0dda8-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="0dda8-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="0dda8-117">Хигхплус</span><span class="sxs-lookup"><span data-stu-id="0dda8-117">highPlus</span></span>|<span data-ttu-id="0dda8-118">2</span><span class="sxs-lookup"><span data-stu-id="0dda8-118">2</span></span>|<span data-ttu-id="0dda8-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="0dda8-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="0dda8-120">Зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="0dda8-120">zeroTolerance</span></span>|<span data-ttu-id="0dda8-121">4</span><span class="sxs-lookup"><span data-stu-id="0dda8-121">3</span></span>|<span data-ttu-id="0dda8-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="0dda8-122">Zero tolerance blocks all unknown executables</span></span>|




