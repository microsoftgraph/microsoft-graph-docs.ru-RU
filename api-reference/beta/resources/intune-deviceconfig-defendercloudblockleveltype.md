---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c00ae796101131456db7206b80e4b6d8999fb86a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729758"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="bbac2-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="bbac2-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="bbac2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbac2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbac2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbac2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbac2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbac2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbac2-107">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="bbac2-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="bbac2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bbac2-108">Members</span></span>
|<span data-ttu-id="bbac2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bbac2-109">Member</span></span>|<span data-ttu-id="bbac2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bbac2-110">Value</span></span>|<span data-ttu-id="bbac2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bbac2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbac2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bbac2-112">notConfigured</span></span>|<span data-ttu-id="bbac2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="bbac2-113">0</span></span>|<span data-ttu-id="bbac2-114">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="bbac2-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="bbac2-115">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="bbac2-115">high</span></span>|<span data-ttu-id="bbac2-116">1,1</span><span class="sxs-lookup"><span data-stu-id="bbac2-116">1</span></span>|<span data-ttu-id="bbac2-117">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="bbac2-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="bbac2-118">хигхплус</span><span class="sxs-lookup"><span data-stu-id="bbac2-118">highPlus</span></span>|<span data-ttu-id="bbac2-119">2</span><span class="sxs-lookup"><span data-stu-id="bbac2-119">2</span></span>|<span data-ttu-id="bbac2-120">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="bbac2-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="bbac2-121">зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="bbac2-121">zeroTolerance</span></span>|<span data-ttu-id="bbac2-122">4</span><span class="sxs-lookup"><span data-stu-id="bbac2-122">3</span></span>|<span data-ttu-id="bbac2-123">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="bbac2-123">Zero tolerance blocks all unknown executables</span></span>|





