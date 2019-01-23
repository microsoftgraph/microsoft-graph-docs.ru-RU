---
title: Тип перечисления folderProtectionType
description: Возможные значения защиты папки
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2abbb719ab93b53ad276f8391d4028c4f8b40b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405718"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="6d084-103">Тип перечисления folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6d084-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="6d084-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6d084-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d084-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d084-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d084-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d084-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d084-107">Возможные значения защиты папки</span><span class="sxs-lookup"><span data-stu-id="6d084-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="6d084-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6d084-108">Members</span></span>
|<span data-ttu-id="6d084-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6d084-109">Member</span></span>|<span data-ttu-id="6d084-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6d084-110">Value</span></span>|<span data-ttu-id="6d084-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6d084-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d084-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="6d084-112">userDefined</span></span>|<span data-ttu-id="6d084-113">0</span><span class="sxs-lookup"><span data-stu-id="6d084-113">0</span></span>|<span data-ttu-id="6d084-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="6d084-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="6d084-115">Включение</span><span class="sxs-lookup"><span data-stu-id="6d084-115">enable</span></span>|<span data-ttu-id="6d084-116">1</span><span class="sxs-lookup"><span data-stu-id="6d084-116">1</span></span>|<span data-ttu-id="6d084-117">Функциональные возможности блока.</span><span class="sxs-lookup"><span data-stu-id="6d084-117">Block functionality.</span></span>|
|<span data-ttu-id="6d084-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="6d084-118">auditMode</span></span>|<span data-ttu-id="6d084-119">2</span><span class="sxs-lookup"><span data-stu-id="6d084-119">2</span></span>|<span data-ttu-id="6d084-120">Разрешить функциональные возможности, но создать журналы.</span><span class="sxs-lookup"><span data-stu-id="6d084-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="6d084-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="6d084-121">blockDiskModification</span></span>|<span data-ttu-id="6d084-122">3</span><span class="sxs-lookup"><span data-stu-id="6d084-122">3</span></span>|<span data-ttu-id="6d084-123">Блокировка ненадежные приложения из записи сектора диска.</span><span class="sxs-lookup"><span data-stu-id="6d084-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="6d084-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="6d084-124">auditDiskModification</span></span>|<span data-ttu-id="6d084-125">4</span><span class="sxs-lookup"><span data-stu-id="6d084-125">4</span></span>|<span data-ttu-id="6d084-126">Создание журналов ненадежные приложения записи сектора диска.</span><span class="sxs-lookup"><span data-stu-id="6d084-126">Generate logs when untrusted apps write to disk sectors.</span></span>|




