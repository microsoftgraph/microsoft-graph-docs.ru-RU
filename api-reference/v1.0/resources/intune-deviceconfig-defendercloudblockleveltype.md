---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575186"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="5234c-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="5234c-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="5234c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5234c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5234c-105">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="5234c-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="5234c-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="5234c-106">Members</span></span>
|<span data-ttu-id="5234c-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="5234c-107">Member</span></span>|<span data-ttu-id="5234c-108">Значение</span><span class="sxs-lookup"><span data-stu-id="5234c-108">Value</span></span>|<span data-ttu-id="5234c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5234c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5234c-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5234c-110">notConfigured</span></span>|<span data-ttu-id="5234c-111">нуль</span><span class="sxs-lookup"><span data-stu-id="5234c-111">0</span></span>|<span data-ttu-id="5234c-112">Значение по умолчанию, используемый по умолчанию уровень блокировки антиВирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="5234c-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="5234c-113">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="5234c-113">high</span></span>|<span data-ttu-id="5234c-114">1 </span><span class="sxs-lookup"><span data-stu-id="5234c-114">1</span></span>|<span data-ttu-id="5234c-115">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="5234c-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="5234c-116">Хигхплус</span><span class="sxs-lookup"><span data-stu-id="5234c-116">highPlus</span></span>|<span data-ttu-id="5234c-117">2 </span><span class="sxs-lookup"><span data-stu-id="5234c-117">2</span></span>|<span data-ttu-id="5234c-118">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="5234c-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="5234c-119">Зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="5234c-119">zeroTolerance</span></span>|<span data-ttu-id="5234c-120">3 </span><span class="sxs-lookup"><span data-stu-id="5234c-120">3</span></span>|<span data-ttu-id="5234c-121">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="5234c-121">Zero tolerance blocks all unknown executables</span></span>|



