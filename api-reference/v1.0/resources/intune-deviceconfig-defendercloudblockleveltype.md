---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 908ebaef963b4c7d8baaf8f1cb0ecfb316d33ad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031880"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="f102d-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="f102d-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="f102d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f102d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f102d-105">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="f102d-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="f102d-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="f102d-106">Members</span></span>
|<span data-ttu-id="f102d-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="f102d-107">Member</span></span>|<span data-ttu-id="f102d-108">Значение</span><span class="sxs-lookup"><span data-stu-id="f102d-108">Value</span></span>|<span data-ttu-id="f102d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f102d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f102d-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f102d-110">notConfigured</span></span>|<span data-ttu-id="f102d-111">нуль</span><span class="sxs-lookup"><span data-stu-id="f102d-111">0</span></span>|<span data-ttu-id="f102d-112">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="f102d-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="f102d-113">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="f102d-113">high</span></span>|<span data-ttu-id="f102d-114">1,1</span><span class="sxs-lookup"><span data-stu-id="f102d-114">1</span></span>|<span data-ttu-id="f102d-115">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="f102d-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="f102d-116">Хигхплус</span><span class="sxs-lookup"><span data-stu-id="f102d-116">highPlus</span></span>|<span data-ttu-id="f102d-117">2</span><span class="sxs-lookup"><span data-stu-id="f102d-117">2</span></span>|<span data-ttu-id="f102d-118">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="f102d-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="f102d-119">Зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="f102d-119">zeroTolerance</span></span>|<span data-ttu-id="f102d-120">4</span><span class="sxs-lookup"><span data-stu-id="f102d-120">3</span></span>|<span data-ttu-id="f102d-121">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="f102d-121">Zero tolerance blocks all unknown executables</span></span>|



