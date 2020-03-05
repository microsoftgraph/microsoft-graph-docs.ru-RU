---
title: тип перечисления Дефендерклаудблокклевелтипе
description: Возможные значения уровня облачного блока
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 381f65c3f9a84c0d126fecd569bab72b48dcfc2a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530186"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="abd99-103">тип перечисления Дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="abd99-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="abd99-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="abd99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abd99-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abd99-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abd99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abd99-107">Возможные значения уровня облачного блока</span><span class="sxs-lookup"><span data-stu-id="abd99-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="abd99-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="abd99-108">Members</span></span>
|<span data-ttu-id="abd99-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="abd99-109">Member</span></span>|<span data-ttu-id="abd99-110">Значение</span><span class="sxs-lookup"><span data-stu-id="abd99-110">Value</span></span>|<span data-ttu-id="abd99-111">Описание</span><span class="sxs-lookup"><span data-stu-id="abd99-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abd99-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="abd99-112">notConfigured</span></span>|<span data-ttu-id="abd99-113">нуль</span><span class="sxs-lookup"><span data-stu-id="abd99-113">0</span></span>|<span data-ttu-id="abd99-114">Значение по умолчанию, используемый по умолчанию уровень блокировки антивирусной программы "Защитник Windows" и обеспечивает строгое обнаружение без увеличения риска обнаружения законных файлов</span><span class="sxs-lookup"><span data-stu-id="abd99-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="abd99-115">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="abd99-115">high</span></span>|<span data-ttu-id="abd99-116">1 </span><span class="sxs-lookup"><span data-stu-id="abd99-116">1</span></span>|<span data-ttu-id="abd99-117">High — применение надежного уровня обнаружения.</span><span class="sxs-lookup"><span data-stu-id="abd99-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="abd99-118">хигхплус</span><span class="sxs-lookup"><span data-stu-id="abd99-118">highPlus</span></span>|<span data-ttu-id="abd99-119">2 </span><span class="sxs-lookup"><span data-stu-id="abd99-119">2</span></span>|<span data-ttu-id="abd99-120">Высокая + использование высокого уровня и применение мер защиты</span><span class="sxs-lookup"><span data-stu-id="abd99-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="abd99-121">зеротолеранце</span><span class="sxs-lookup"><span data-stu-id="abd99-121">zeroTolerance</span></span>|<span data-ttu-id="abd99-122">3 </span><span class="sxs-lookup"><span data-stu-id="abd99-122">3</span></span>|<span data-ttu-id="abd99-123">Нулевое отклонение блокирует все неизвестные исполняемые файлы</span><span class="sxs-lookup"><span data-stu-id="abd99-123">Zero tolerance blocks all unknown executables</span></span>|



