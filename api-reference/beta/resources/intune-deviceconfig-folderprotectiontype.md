---
title: Тип перечисления folderProtectionType
description: Возможные значения защиты папки
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 427bdb4fcb93a831ab120aa0c7eefcbf97675fa8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973754"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="fcdfd-103">Тип перечисления folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="fcdfd-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="fcdfd-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fcdfd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcdfd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcdfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcdfd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fcdfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcdfd-107">Возможные значения защиты папки</span><span class="sxs-lookup"><span data-stu-id="fcdfd-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="fcdfd-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fcdfd-108">Members</span></span>
|<span data-ttu-id="fcdfd-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fcdfd-109">Member</span></span>|<span data-ttu-id="fcdfd-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fcdfd-110">Value</span></span>|<span data-ttu-id="fcdfd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fcdfd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcdfd-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="fcdfd-112">userDefined</span></span>|<span data-ttu-id="fcdfd-113">0</span><span class="sxs-lookup"><span data-stu-id="fcdfd-113">0</span></span>|<span data-ttu-id="fcdfd-114">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="fcdfd-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="fcdfd-115">Включение</span><span class="sxs-lookup"><span data-stu-id="fcdfd-115">enable</span></span>|<span data-ttu-id="fcdfd-116">1</span><span class="sxs-lookup"><span data-stu-id="fcdfd-116">1</span></span>|<span data-ttu-id="fcdfd-117">Функциональные возможности блока.</span><span class="sxs-lookup"><span data-stu-id="fcdfd-117">Block functionality.</span></span>|
|<span data-ttu-id="fcdfd-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="fcdfd-118">auditMode</span></span>|<span data-ttu-id="fcdfd-119">2</span><span class="sxs-lookup"><span data-stu-id="fcdfd-119">2</span></span>|<span data-ttu-id="fcdfd-120">Разрешить функциональные возможности, но создать журналы.</span><span class="sxs-lookup"><span data-stu-id="fcdfd-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="fcdfd-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="fcdfd-121">blockDiskModification</span></span>|<span data-ttu-id="fcdfd-122">3</span><span class="sxs-lookup"><span data-stu-id="fcdfd-122">3</span></span>|<span data-ttu-id="fcdfd-123">Блокировка ненадежные приложения из записи сектора диска.</span><span class="sxs-lookup"><span data-stu-id="fcdfd-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="fcdfd-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="fcdfd-124">auditDiskModification</span></span>|<span data-ttu-id="fcdfd-125">4</span><span class="sxs-lookup"><span data-stu-id="fcdfd-125">4</span></span>|<span data-ttu-id="fcdfd-126">Создание журналов ненадежные приложения записи сектора диска.</span><span class="sxs-lookup"><span data-stu-id="fcdfd-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





