---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 86d3da357b519ab3da0e4a4947ab933339aae134
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449091"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="d0dbb-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="d0dbb-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="d0dbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0dbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0dbb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0dbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0dbb-106">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="d0dbb-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="d0dbb-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d0dbb-107">Members</span></span>
|<span data-ttu-id="d0dbb-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d0dbb-108">Member</span></span>|<span data-ttu-id="d0dbb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d0dbb-109">Value</span></span>|<span data-ttu-id="d0dbb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0dbb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0dbb-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d0dbb-111">notConfigured</span></span>|<span data-ttu-id="d0dbb-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d0dbb-112">0</span></span>|<span data-ttu-id="d0dbb-113">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="d0dbb-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="d0dbb-114">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="d0dbb-114">high</span></span>|<span data-ttu-id="d0dbb-115">1,1</span><span class="sxs-lookup"><span data-stu-id="d0dbb-115">1</span></span>|<span data-ttu-id="d0dbb-116">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="d0dbb-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="d0dbb-117">хигхплус</span><span class="sxs-lookup"><span data-stu-id="d0dbb-117">highPlus</span></span>|<span data-ttu-id="d0dbb-118">2</span><span class="sxs-lookup"><span data-stu-id="d0dbb-118">2</span></span>|<span data-ttu-id="d0dbb-119">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="d0dbb-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="d0dbb-120">зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="d0dbb-120">zeroTolerance</span></span>|<span data-ttu-id="d0dbb-121">4</span><span class="sxs-lookup"><span data-stu-id="d0dbb-121">3</span></span>|<span data-ttu-id="d0dbb-122">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="d0dbb-122">Zero tolerance blocks all unknown executables</span></span>|







