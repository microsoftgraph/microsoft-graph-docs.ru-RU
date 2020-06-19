---
title: тип перечисления win32LobAppFileSystemOperationType
description: Содержит все поддерживаемые типы обнаружения файловой системы.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8e1224388b988eb0bab7286f14a21111b75daa8a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790840"
---
# <a name="win32lobappfilesystemoperationtype-enum-type"></a><span data-ttu-id="ef25a-103">тип перечисления win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="ef25a-103">win32LobAppFileSystemOperationType enum type</span></span>

<span data-ttu-id="ef25a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef25a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef25a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef25a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef25a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef25a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef25a-107">Содержит все поддерживаемые типы обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="ef25a-107">Contains all supported file system detection type.</span></span>

## <a name="members"></a><span data-ttu-id="ef25a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ef25a-108">Members</span></span>
|<span data-ttu-id="ef25a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ef25a-109">Member</span></span>|<span data-ttu-id="ef25a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ef25a-110">Value</span></span>|<span data-ttu-id="ef25a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ef25a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef25a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ef25a-112">notConfigured</span></span>|<span data-ttu-id="ef25a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ef25a-113">0</span></span>|<span data-ttu-id="ef25a-114">Не настроен.</span><span class="sxs-lookup"><span data-stu-id="ef25a-114">Not configured.</span></span>|
|<span data-ttu-id="ef25a-115">Существует</span><span class="sxs-lookup"><span data-stu-id="ef25a-115">exists</span></span>|<span data-ttu-id="ef25a-116">1 </span><span class="sxs-lookup"><span data-stu-id="ef25a-116">1</span></span>|<span data-ttu-id="ef25a-117">Существует ли указанный файл или папка.</span><span class="sxs-lookup"><span data-stu-id="ef25a-117">Whether the specified file or folder exists.</span></span>|
|<span data-ttu-id="ef25a-118">modifiedDate</span><span class="sxs-lookup"><span data-stu-id="ef25a-118">modifiedDate</span></span>|<span data-ttu-id="ef25a-119">2</span><span class="sxs-lookup"><span data-stu-id="ef25a-119">2</span></span>|<span data-ttu-id="ef25a-120">Дата последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="ef25a-120">Last modified date.</span></span>|
|<span data-ttu-id="ef25a-121">createdDate</span><span class="sxs-lookup"><span data-stu-id="ef25a-121">createdDate</span></span>|<span data-ttu-id="ef25a-122">4</span><span class="sxs-lookup"><span data-stu-id="ef25a-122">3</span></span>|<span data-ttu-id="ef25a-123">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="ef25a-123">Created date.</span></span>|
|<span data-ttu-id="ef25a-124">version</span><span class="sxs-lookup"><span data-stu-id="ef25a-124">version</span></span>|<span data-ttu-id="ef25a-125">4 </span><span class="sxs-lookup"><span data-stu-id="ef25a-125">4</span></span>|<span data-ttu-id="ef25a-126">Тип значения Version.</span><span class="sxs-lookup"><span data-stu-id="ef25a-126">Version value type.</span></span>|
|<span data-ttu-id="ef25a-127">сизеинмб</span><span class="sxs-lookup"><span data-stu-id="ef25a-127">sizeInMB</span></span>|<span data-ttu-id="ef25a-128">5 </span><span class="sxs-lookup"><span data-stu-id="ef25a-128">5</span></span>|<span data-ttu-id="ef25a-129">Тип определения размера.</span><span class="sxs-lookup"><span data-stu-id="ef25a-129">Size detection type.</span></span>|
|<span data-ttu-id="ef25a-130">доеснотексист</span><span class="sxs-lookup"><span data-stu-id="ef25a-130">doesNotExist</span></span>|<span data-ttu-id="ef25a-131">6 </span><span class="sxs-lookup"><span data-stu-id="ef25a-131">6</span></span>|<span data-ttu-id="ef25a-132">Указанный файл или папка не существует.</span><span class="sxs-lookup"><span data-stu-id="ef25a-132">The specified file or folder does not exist.</span></span>|



