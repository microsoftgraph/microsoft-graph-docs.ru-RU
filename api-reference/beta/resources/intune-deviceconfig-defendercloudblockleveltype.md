---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc0e99f9d964e80410b10bc48e20ea0a5fd1d608
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333592"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="da9f5-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="da9f5-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="da9f5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da9f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da9f5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da9f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da9f5-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="da9f5-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="da9f5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="da9f5-107">Members</span></span>
|<span data-ttu-id="da9f5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="da9f5-108">Member</span></span>|<span data-ttu-id="da9f5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="da9f5-109">Value</span></span>|<span data-ttu-id="da9f5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="da9f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da9f5-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="da9f5-111">notConfigured</span></span>|<span data-ttu-id="da9f5-112">нуль</span><span class="sxs-lookup"><span data-stu-id="da9f5-112">0</span></span>|<span data-ttu-id="da9f5-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="da9f5-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="da9f5-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="da9f5-114">high</span></span>|<span data-ttu-id="da9f5-115">1,1</span><span class="sxs-lookup"><span data-stu-id="da9f5-115">1</span></span>|<span data-ttu-id="da9f5-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="da9f5-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="da9f5-117">хигхплус</span><span class="sxs-lookup"><span data-stu-id="da9f5-117">highPlus</span></span>|<span data-ttu-id="da9f5-118">2</span><span class="sxs-lookup"><span data-stu-id="da9f5-118">2</span></span>|<span data-ttu-id="da9f5-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="da9f5-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="da9f5-120">зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="da9f5-120">zeroTolerance</span></span>|<span data-ttu-id="da9f5-121">4</span><span class="sxs-lookup"><span data-stu-id="da9f5-121">3</span></span>|<span data-ttu-id="da9f5-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="da9f5-122">Zero tolerance blocks all unknown executables</span></span>|



