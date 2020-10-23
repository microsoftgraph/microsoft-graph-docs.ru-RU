---
title: тип перечисления win32LobAppFileSystemDetectionType
description: Содержит все поддерживаемые типы обнаружения файловой системы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 68136da5618db38c4ac44edf2a42741867ff86f9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696414"
---
# <a name="win32lobappfilesystemdetectiontype-enum-type"></a><span data-ttu-id="8b365-103">тип перечисления win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="8b365-103">win32LobAppFileSystemDetectionType enum type</span></span>

<span data-ttu-id="8b365-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b365-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b365-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b365-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b365-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b365-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b365-107">Содержит все поддерживаемые типы обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="8b365-107">Contains all supported file system detection type.</span></span>

## <a name="members"></a><span data-ttu-id="8b365-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8b365-108">Members</span></span>
|<span data-ttu-id="8b365-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8b365-109">Member</span></span>|<span data-ttu-id="8b365-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8b365-110">Value</span></span>|<span data-ttu-id="8b365-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8b365-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b365-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8b365-112">notConfigured</span></span>|<span data-ttu-id="8b365-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8b365-113">0</span></span>|<span data-ttu-id="8b365-114">Не настроен.</span><span class="sxs-lookup"><span data-stu-id="8b365-114">Not configured.</span></span>|
|<span data-ttu-id="8b365-115">Существует</span><span class="sxs-lookup"><span data-stu-id="8b365-115">exists</span></span>|<span data-ttu-id="8b365-116">1,1</span><span class="sxs-lookup"><span data-stu-id="8b365-116">1</span></span>|<span data-ttu-id="8b365-117">Существует ли указанный файл или папка.</span><span class="sxs-lookup"><span data-stu-id="8b365-117">Whether the specified file or folder exists.</span></span>|
|<span data-ttu-id="8b365-118">modifiedDate</span><span class="sxs-lookup"><span data-stu-id="8b365-118">modifiedDate</span></span>|<span data-ttu-id="8b365-119">2</span><span class="sxs-lookup"><span data-stu-id="8b365-119">2</span></span>|<span data-ttu-id="8b365-120">Дата последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="8b365-120">Last modified date.</span></span>|
|<span data-ttu-id="8b365-121">createdDate</span><span class="sxs-lookup"><span data-stu-id="8b365-121">createdDate</span></span>|<span data-ttu-id="8b365-122">4</span><span class="sxs-lookup"><span data-stu-id="8b365-122">3</span></span>|<span data-ttu-id="8b365-123">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="8b365-123">Created date.</span></span>|
|<span data-ttu-id="8b365-124">version</span><span class="sxs-lookup"><span data-stu-id="8b365-124">version</span></span>|<span data-ttu-id="8b365-125">4 </span><span class="sxs-lookup"><span data-stu-id="8b365-125">4</span></span>|<span data-ttu-id="8b365-126">Тип значения Version.</span><span class="sxs-lookup"><span data-stu-id="8b365-126">Version value type.</span></span>|
|<span data-ttu-id="8b365-127">сизеинмб</span><span class="sxs-lookup"><span data-stu-id="8b365-127">sizeInMB</span></span>|<span data-ttu-id="8b365-128">5 </span><span class="sxs-lookup"><span data-stu-id="8b365-128">5</span></span>|<span data-ttu-id="8b365-129">Тип определения размера.</span><span class="sxs-lookup"><span data-stu-id="8b365-129">Size detection type.</span></span>|
|<span data-ttu-id="8b365-130">доеснотексист</span><span class="sxs-lookup"><span data-stu-id="8b365-130">doesNotExist</span></span>|<span data-ttu-id="8b365-131">6 </span><span class="sxs-lookup"><span data-stu-id="8b365-131">6</span></span>|<span data-ttu-id="8b365-132">Указанный файл или папка не существует.</span><span class="sxs-lookup"><span data-stu-id="8b365-132">The specified file or folder does not exist.</span></span>|





