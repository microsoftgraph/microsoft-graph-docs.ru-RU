---
title: тип перечисления Фолдерпротектионтипе
description: Возможные значения защиты папок
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 741565678be1bfb533c4445c02c767f87fdfca05
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556090"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="cfba9-103">тип перечисления Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="cfba9-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="cfba9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfba9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfba9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfba9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfba9-106">Возможные значения защиты папок</span><span class="sxs-lookup"><span data-stu-id="cfba9-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="cfba9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cfba9-107">Members</span></span>
|<span data-ttu-id="cfba9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cfba9-108">Member</span></span>|<span data-ttu-id="cfba9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cfba9-109">Value</span></span>|<span data-ttu-id="cfba9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cfba9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfba9-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="cfba9-111">userDefined</span></span>|<span data-ttu-id="cfba9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cfba9-112">0</span></span>|<span data-ttu-id="cfba9-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="cfba9-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="cfba9-114">подключить</span><span class="sxs-lookup"><span data-stu-id="cfba9-114">enable</span></span>|<span data-ttu-id="cfba9-115">1 </span><span class="sxs-lookup"><span data-stu-id="cfba9-115">1</span></span>|<span data-ttu-id="cfba9-116">Функциональная возможность блока.</span><span class="sxs-lookup"><span data-stu-id="cfba9-116">Block functionality.</span></span>|
|<span data-ttu-id="cfba9-117">Аудитмоде</span><span class="sxs-lookup"><span data-stu-id="cfba9-117">auditMode</span></span>|<span data-ttu-id="cfba9-118">2 </span><span class="sxs-lookup"><span data-stu-id="cfba9-118">2</span></span>|<span data-ttu-id="cfba9-119">РазРешите функциональные возможности, но Создайте журналы.</span><span class="sxs-lookup"><span data-stu-id="cfba9-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="cfba9-120">Блоккдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="cfba9-120">blockDiskModification</span></span>|<span data-ttu-id="cfba9-121">3 </span><span class="sxs-lookup"><span data-stu-id="cfba9-121">3</span></span>|<span data-ttu-id="cfba9-122">Блокировать запись недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="cfba9-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="cfba9-123">Аудитдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="cfba9-123">auditDiskModification</span></span>|<span data-ttu-id="cfba9-124">4 </span><span class="sxs-lookup"><span data-stu-id="cfba9-124">4</span></span>|<span data-ttu-id="cfba9-125">Создание журналов при записи недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="cfba9-125">Generate logs when untrusted apps write to disk sectors.</span></span>|





