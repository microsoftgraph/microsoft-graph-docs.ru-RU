---
title: тип перечисления Граупполициуплоадеддефинитионфилестатус
description: Тип групповой политики передал состояние файла определения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 70430e74d332baf0b1c81a41d2098883688464ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030614"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a><span data-ttu-id="24976-103">тип перечисления Граупполициуплоадеддефинитионфилестатус</span><span class="sxs-lookup"><span data-stu-id="24976-103">groupPolicyUploadedDefinitionFileStatus enum type</span></span>

<span data-ttu-id="24976-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24976-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24976-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24976-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24976-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24976-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24976-107">Тип групповой политики передал состояние файла определения.</span><span class="sxs-lookup"><span data-stu-id="24976-107">Type of Group Policy uploaded definition file status.</span></span>

## <a name="members"></a><span data-ttu-id="24976-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="24976-108">Members</span></span>
|<span data-ttu-id="24976-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="24976-109">Member</span></span>|<span data-ttu-id="24976-110">Значение</span><span class="sxs-lookup"><span data-stu-id="24976-110">Value</span></span>|<span data-ttu-id="24976-111">Описание</span><span class="sxs-lookup"><span data-stu-id="24976-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24976-112">Нет</span><span class="sxs-lookup"><span data-stu-id="24976-112">none</span></span>|<span data-ttu-id="24976-113">нуль</span><span class="sxs-lookup"><span data-stu-id="24976-113">0</span></span>|<span data-ttu-id="24976-114">Групповая политика загружена файл определения Недопустимый статус отправки.</span><span class="sxs-lookup"><span data-stu-id="24976-114">Group Policy uploaded definition file invalid upload status.</span></span>|
|<span data-ttu-id="24976-115">уплоадинпрогресс</span><span class="sxs-lookup"><span data-stu-id="24976-115">uploadInProgress</span></span>|<span data-ttu-id="24976-116">1 </span><span class="sxs-lookup"><span data-stu-id="24976-116">1</span></span>|<span data-ttu-id="24976-117">Групповая политика перегрузила файл определения, выполняется отправка.</span><span class="sxs-lookup"><span data-stu-id="24976-117">Group Policy uploaded definition file upload in progress.</span></span>|
|<span data-ttu-id="24976-118">доступен</span><span class="sxs-lookup"><span data-stu-id="24976-118">available</span></span>|<span data-ttu-id="24976-119">2 </span><span class="sxs-lookup"><span data-stu-id="24976-119">2</span></span>|<span data-ttu-id="24976-120">Групповая политика загрузила доступный файл определения.</span><span class="sxs-lookup"><span data-stu-id="24976-120">Group Policy uploaded definition file available.</span></span>|
|<span data-ttu-id="24976-121">ей</span><span class="sxs-lookup"><span data-stu-id="24976-121">assigned</span></span>|<span data-ttu-id="24976-122">4</span><span class="sxs-lookup"><span data-stu-id="24976-122">3</span></span>|<span data-ttu-id="24976-123">Групповая политика загрузила файл определения, назначенный политике.</span><span class="sxs-lookup"><span data-stu-id="24976-123">Group Policy uploaded definition file assigned to policy.</span></span>|
|<span data-ttu-id="24976-124">ремовалинпрогресс</span><span class="sxs-lookup"><span data-stu-id="24976-124">removalInProgress</span></span>|<span data-ttu-id="24976-125">4 </span><span class="sxs-lookup"><span data-stu-id="24976-125">4</span></span>|<span data-ttu-id="24976-126">Групповая политика перегрузила файл определения, который выполняется удаление.</span><span class="sxs-lookup"><span data-stu-id="24976-126">Group Policy uploaded definition file removal in progress.</span></span>|
|<span data-ttu-id="24976-127">уплоадфаилед</span><span class="sxs-lookup"><span data-stu-id="24976-127">uploadFailed</span></span>|<span data-ttu-id="24976-128">5 </span><span class="sxs-lookup"><span data-stu-id="24976-128">5</span></span>|<span data-ttu-id="24976-129">Групповая политика загружена не удалось отправить файл определения.</span><span class="sxs-lookup"><span data-stu-id="24976-129">Group Policy uploaded definition file upload failed.</span></span>|
|<span data-ttu-id="24976-130">ремовалфаилед</span><span class="sxs-lookup"><span data-stu-id="24976-130">removalFailed</span></span>|<span data-ttu-id="24976-131">6 </span><span class="sxs-lookup"><span data-stu-id="24976-131">6</span></span>|<span data-ttu-id="24976-132">Групповая политика перезагружена. не удалось удалить файл определения.</span><span class="sxs-lookup"><span data-stu-id="24976-132">Group Policy uploaded definition file removal failed.</span></span>|






