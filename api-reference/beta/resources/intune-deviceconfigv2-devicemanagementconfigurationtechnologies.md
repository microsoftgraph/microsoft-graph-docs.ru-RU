---
title: тип enum deviceManagementConfigurationTechnologies
description: Описывает, какую технологию можно развернуть с помощью этого параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b0e6a6324f9157fb528fd5aeb7772f4c1e8721fe
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666697"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a><span data-ttu-id="85c8d-103">тип enum deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="85c8d-103">deviceManagementConfigurationTechnologies enum type</span></span>

<span data-ttu-id="85c8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85c8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85c8d-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85c8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85c8d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85c8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85c8d-107">Описывает, какую технологию можно развернуть с помощью этого параметра</span><span class="sxs-lookup"><span data-stu-id="85c8d-107">Describes which technology this setting can be deployed with</span></span>

## <a name="members"></a><span data-ttu-id="85c8d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="85c8d-108">Members</span></span>
|<span data-ttu-id="85c8d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="85c8d-109">Member</span></span>|<span data-ttu-id="85c8d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="85c8d-110">Value</span></span>|<span data-ttu-id="85c8d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85c8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85c8d-112">нет</span><span class="sxs-lookup"><span data-stu-id="85c8d-112">none</span></span>|<span data-ttu-id="85c8d-113">0</span><span class="sxs-lookup"><span data-stu-id="85c8d-113">0</span></span>|<span data-ttu-id="85c8d-114">Настройка не может быть развернута по любому каналу</span><span class="sxs-lookup"><span data-stu-id="85c8d-114">Setting cannot be deployed through any channel</span></span>|
|<span data-ttu-id="85c8d-115">mdm</span><span class="sxs-lookup"><span data-stu-id="85c8d-115">mdm</span></span>|<span data-ttu-id="85c8d-116">1</span><span class="sxs-lookup"><span data-stu-id="85c8d-116">1</span></span>|<span data-ttu-id="85c8d-117">Параметр можно развернуть через канал MDM</span><span class="sxs-lookup"><span data-stu-id="85c8d-117">Setting can be deployed through the MDM channel</span></span>|
|<span data-ttu-id="85c8d-118">windows10XManagement</span><span class="sxs-lookup"><span data-stu-id="85c8d-118">windows10XManagement</span></span>|<span data-ttu-id="85c8d-119">2</span><span class="sxs-lookup"><span data-stu-id="85c8d-119">2</span></span>|<span data-ttu-id="85c8d-120">Параметр можно развернуть через канал Windows10XManagement</span><span class="sxs-lookup"><span data-stu-id="85c8d-120">Setting can be deployed through the Windows10XManagement channel</span></span>|
|<span data-ttu-id="85c8d-121">configManager</span><span class="sxs-lookup"><span data-stu-id="85c8d-121">configManager</span></span>|<span data-ttu-id="85c8d-122">4 </span><span class="sxs-lookup"><span data-stu-id="85c8d-122">4</span></span>|<span data-ttu-id="85c8d-123">Параметр можно развернуть через канал ConfigManager</span><span class="sxs-lookup"><span data-stu-id="85c8d-123">Setting can be deployed through the ConfigManager channel</span></span>|
|<span data-ttu-id="85c8d-124">MicrosoftSense</span><span class="sxs-lookup"><span data-stu-id="85c8d-124">microsoftSense</span></span>|<span data-ttu-id="85c8d-125">128</span><span class="sxs-lookup"><span data-stu-id="85c8d-125">128</span></span>|<span data-ttu-id="85c8d-126">Настройка может быть развернута через канал агента SENSE</span><span class="sxs-lookup"><span data-stu-id="85c8d-126">Setting can be deployed through the SENSE agent channel</span></span>|




