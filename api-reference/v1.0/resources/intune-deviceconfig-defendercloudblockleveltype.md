---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258837"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="dfa04-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="dfa04-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="dfa04-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfa04-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfa04-105">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="dfa04-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="dfa04-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="dfa04-106">Members</span></span>
|<span data-ttu-id="dfa04-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="dfa04-107">Member</span></span>|<span data-ttu-id="dfa04-108">Значение</span><span class="sxs-lookup"><span data-stu-id="dfa04-108">Value</span></span>|<span data-ttu-id="dfa04-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa04-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfa04-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="dfa04-110">notConfigured</span></span>|<span data-ttu-id="dfa04-111">нуль</span><span class="sxs-lookup"><span data-stu-id="dfa04-111">0</span></span>|<span data-ttu-id="dfa04-112">Значение по умолчанию, используемый по умолчанию уровень блокировки антиВирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="dfa04-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="dfa04-113">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="dfa04-113">high</span></span>|<span data-ttu-id="dfa04-114">1,1</span><span class="sxs-lookup"><span data-stu-id="dfa04-114">1</span></span>|<span data-ttu-id="dfa04-115">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="dfa04-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="dfa04-116">Хигхплус</span><span class="sxs-lookup"><span data-stu-id="dfa04-116">highPlus</span></span>|<span data-ttu-id="dfa04-117">2</span><span class="sxs-lookup"><span data-stu-id="dfa04-117">2</span></span>|<span data-ttu-id="dfa04-118">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="dfa04-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="dfa04-119">Зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="dfa04-119">zeroTolerance</span></span>|<span data-ttu-id="dfa04-120">4</span><span class="sxs-lookup"><span data-stu-id="dfa04-120">3</span></span>|<span data-ttu-id="dfa04-121">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="dfa04-121">Zero tolerance blocks all unknown executables</span></span>|



