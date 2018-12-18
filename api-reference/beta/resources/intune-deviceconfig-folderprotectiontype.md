---
title: Тип перечисления folderProtectionType
description: Возможные значения защиты папки
author: tfitzmac
ms.openlocfilehash: 93df62da9bb5d849cba86b52384f45bfe7bd760f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350605"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="0d768-103">Тип перечисления folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="0d768-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="0d768-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d768-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d768-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d768-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d768-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0d768-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d768-107">Возможные значения защиты папки</span><span class="sxs-lookup"><span data-stu-id="0d768-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="0d768-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0d768-108">Members</span></span>
|<span data-ttu-id="0d768-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0d768-109">Member</span></span>|<span data-ttu-id="0d768-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0d768-110">Value</span></span>|<span data-ttu-id="0d768-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d768-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d768-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="0d768-112">userDefined</span></span>|<span data-ttu-id="0d768-113">0</span><span class="sxs-lookup"><span data-stu-id="0d768-113">0</span></span>|<span data-ttu-id="0d768-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="0d768-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="0d768-115">Включение</span><span class="sxs-lookup"><span data-stu-id="0d768-115">enable</span></span>|<span data-ttu-id="0d768-116">1</span><span class="sxs-lookup"><span data-stu-id="0d768-116">1</span></span>|<span data-ttu-id="0d768-117">Функциональные возможности блока.</span><span class="sxs-lookup"><span data-stu-id="0d768-117">Block functionality.</span></span>|
|<span data-ttu-id="0d768-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="0d768-118">auditMode</span></span>|<span data-ttu-id="0d768-119">2</span><span class="sxs-lookup"><span data-stu-id="0d768-119">2</span></span>|<span data-ttu-id="0d768-120">Разрешить функциональные возможности, но создать журналы.</span><span class="sxs-lookup"><span data-stu-id="0d768-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="0d768-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="0d768-121">blockDiskModification</span></span>|<span data-ttu-id="0d768-122">3</span><span class="sxs-lookup"><span data-stu-id="0d768-122">3</span></span>|<span data-ttu-id="0d768-123">Блокировка ненадежные приложения из записи сектора диска.</span><span class="sxs-lookup"><span data-stu-id="0d768-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="0d768-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="0d768-124">auditDiskModification</span></span>|<span data-ttu-id="0d768-125">4</span><span class="sxs-lookup"><span data-stu-id="0d768-125">4</span></span>|<span data-ttu-id="0d768-126">Создание журналов ненадежные приложения записи сектора диска.</span><span class="sxs-lookup"><span data-stu-id="0d768-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





