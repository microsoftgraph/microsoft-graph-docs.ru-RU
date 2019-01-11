---
title: Тип ресурса windowsInformationProtectionDesktopApp
description: Защита данных классических приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c381541379feacff7611e77882069c5fe2119e67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822066"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="ef585-103">Тип ресурса windowsInformationProtectionDesktopApp</span><span class="sxs-lookup"><span data-stu-id="ef585-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="ef585-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ef585-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef585-105">Защита данных классических приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="ef585-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="ef585-106">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="ef585-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ef585-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef585-107">Properties</span></span>
|<span data-ttu-id="ef585-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef585-108">Property</span></span>|<span data-ttu-id="ef585-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ef585-109">Type</span></span>|<span data-ttu-id="ef585-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef585-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef585-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ef585-111">displayName</span></span>|<span data-ttu-id="ef585-112">String</span><span class="sxs-lookup"><span data-stu-id="ef585-112">String</span></span>|<span data-ttu-id="ef585-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="ef585-113">App display name.</span></span> <span data-ttu-id="ef585-114">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="ef585-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="ef585-115">описание</span><span class="sxs-lookup"><span data-stu-id="ef585-115">description</span></span>|<span data-ttu-id="ef585-116">String</span><span class="sxs-lookup"><span data-stu-id="ef585-116">String</span></span>|<span data-ttu-id="ef585-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ef585-117">The app's description.</span></span> <span data-ttu-id="ef585-118">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="ef585-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="ef585-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="ef585-119">publisherName</span></span>|<span data-ttu-id="ef585-120">String</span><span class="sxs-lookup"><span data-stu-id="ef585-120">String</span></span>|<span data-ttu-id="ef585-121">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="ef585-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="ef585-122">productName</span><span class="sxs-lookup"><span data-stu-id="ef585-122">productName</span></span>|<span data-ttu-id="ef585-123">String</span><span class="sxs-lookup"><span data-stu-id="ef585-123">String</span></span>|<span data-ttu-id="ef585-124">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="ef585-124">The product name.</span></span> <span data-ttu-id="ef585-125">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="ef585-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="ef585-126">denied</span><span class="sxs-lookup"><span data-stu-id="ef585-126">denied</span></span>|<span data-ttu-id="ef585-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef585-127">Boolean</span></span>|<span data-ttu-id="ef585-128">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="ef585-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="ef585-129">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="ef585-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="ef585-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="ef585-130">binaryName</span></span>|<span data-ttu-id="ef585-131">String</span><span class="sxs-lookup"><span data-stu-id="ef585-131">String</span></span>|<span data-ttu-id="ef585-132">Двоичное имя.</span><span class="sxs-lookup"><span data-stu-id="ef585-132">The binary name.</span></span>|
|<span data-ttu-id="ef585-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="ef585-133">binaryVersionLow</span></span>|<span data-ttu-id="ef585-134">String</span><span class="sxs-lookup"><span data-stu-id="ef585-134">String</span></span>|<span data-ttu-id="ef585-135">Нижняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="ef585-135">The lower binary version.</span></span>|
|<span data-ttu-id="ef585-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="ef585-136">binaryVersionHigh</span></span>|<span data-ttu-id="ef585-137">String</span><span class="sxs-lookup"><span data-stu-id="ef585-137">String</span></span>|<span data-ttu-id="ef585-138">Верхняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="ef585-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef585-139">Связи</span><span class="sxs-lookup"><span data-stu-id="ef585-139">Relationships</span></span>
<span data-ttu-id="ef585-140">Нет</span><span class="sxs-lookup"><span data-stu-id="ef585-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ef585-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef585-141">JSON Representation</span></span>
<span data-ttu-id="ef585-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef585-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



