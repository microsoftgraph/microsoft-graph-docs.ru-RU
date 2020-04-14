---
title: тип перечисления Граупполициуплоадеддефинитионфилестатус
description: Тип групповой политики передал состояние файла определения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 902741b134b8661786892c5c722a79b013fc1126
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385943"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a><span data-ttu-id="9bfd5-103">тип перечисления Граупполициуплоадеддефинитионфилестатус</span><span class="sxs-lookup"><span data-stu-id="9bfd5-103">groupPolicyUploadedDefinitionFileStatus enum type</span></span>

<span data-ttu-id="9bfd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bfd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bfd5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bfd5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bfd5-107">Тип групповой политики передал состояние файла определения.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-107">Type of Group Policy uploaded definition file status.</span></span>

## <a name="members"></a><span data-ttu-id="9bfd5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9bfd5-108">Members</span></span>
|<span data-ttu-id="9bfd5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9bfd5-109">Member</span></span>|<span data-ttu-id="9bfd5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9bfd5-110">Value</span></span>|<span data-ttu-id="9bfd5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9bfd5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bfd5-112">нет</span><span class="sxs-lookup"><span data-stu-id="9bfd5-112">none</span></span>|<span data-ttu-id="9bfd5-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9bfd5-113">0</span></span>|<span data-ttu-id="9bfd5-114">Групповая политика загружена файл определения Недопустимый статус отправки.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-114">Group Policy uploaded definition file invalid upload status.</span></span>|
|<span data-ttu-id="9bfd5-115">уплоадинпрогресс</span><span class="sxs-lookup"><span data-stu-id="9bfd5-115">uploadInProgress</span></span>|<span data-ttu-id="9bfd5-116">1,1</span><span class="sxs-lookup"><span data-stu-id="9bfd5-116">1</span></span>|<span data-ttu-id="9bfd5-117">Групповая политика перегрузила файл определения, выполняется отправка.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-117">Group Policy uploaded definition file upload in progress.</span></span>|
|<span data-ttu-id="9bfd5-118">доступен</span><span class="sxs-lookup"><span data-stu-id="9bfd5-118">available</span></span>|<span data-ttu-id="9bfd5-119">2</span><span class="sxs-lookup"><span data-stu-id="9bfd5-119">2</span></span>|<span data-ttu-id="9bfd5-120">Групповая политика загрузила доступный файл определения.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-120">Group Policy uploaded definition file available.</span></span>|
|<span data-ttu-id="9bfd5-121">ей</span><span class="sxs-lookup"><span data-stu-id="9bfd5-121">assigned</span></span>|<span data-ttu-id="9bfd5-122">4</span><span class="sxs-lookup"><span data-stu-id="9bfd5-122">3</span></span>|<span data-ttu-id="9bfd5-123">Групповая политика загрузила файл определения, назначенный политике.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-123">Group Policy uploaded definition file assigned to policy.</span></span>|
|<span data-ttu-id="9bfd5-124">ремовалинпрогресс</span><span class="sxs-lookup"><span data-stu-id="9bfd5-124">removalInProgress</span></span>|<span data-ttu-id="9bfd5-125">4 </span><span class="sxs-lookup"><span data-stu-id="9bfd5-125">4</span></span>|<span data-ttu-id="9bfd5-126">Групповая политика перегрузила файл определения, который выполняется удаление.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-126">Group Policy uploaded definition file removal in progress.</span></span>|
|<span data-ttu-id="9bfd5-127">уплоадфаилед</span><span class="sxs-lookup"><span data-stu-id="9bfd5-127">uploadFailed</span></span>|<span data-ttu-id="9bfd5-128">5 </span><span class="sxs-lookup"><span data-stu-id="9bfd5-128">5</span></span>|<span data-ttu-id="9bfd5-129">Групповая политика загружена не удалось отправить файл определения.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-129">Group Policy uploaded definition file upload failed.</span></span>|
|<span data-ttu-id="9bfd5-130">ремовалфаилед</span><span class="sxs-lookup"><span data-stu-id="9bfd5-130">removalFailed</span></span>|<span data-ttu-id="9bfd5-131">6 </span><span class="sxs-lookup"><span data-stu-id="9bfd5-131">6</span></span>|<span data-ttu-id="9bfd5-132">Групповая политика перезагружена. не удалось удалить файл определения.</span><span class="sxs-lookup"><span data-stu-id="9bfd5-132">Group Policy uploaded definition file removal failed.</span></span>|



