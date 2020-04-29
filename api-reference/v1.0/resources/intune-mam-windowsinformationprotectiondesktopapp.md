---
title: Тип ресурса windowsInformationProtectionDesktopApp
description: Защита данных классических приложений для Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e962733cb062a2eab2faaa521b567af65e6e5483
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468413"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="a867b-103">Тип ресурса windowsInformationProtectionDesktopApp</span><span class="sxs-lookup"><span data-stu-id="a867b-103">windowsInformationProtectionDesktopApp resource type</span></span>

<span data-ttu-id="a867b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a867b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a867b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a867b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a867b-106">Защита данных классических приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="a867b-106">Desktop App for Windows information protection</span></span>


<span data-ttu-id="a867b-107">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a867b-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a867b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a867b-108">Properties</span></span>
|<span data-ttu-id="a867b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a867b-109">Property</span></span>|<span data-ttu-id="a867b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a867b-110">Type</span></span>|<span data-ttu-id="a867b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a867b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a867b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a867b-112">displayName</span></span>|<span data-ttu-id="a867b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a867b-113">String</span></span>|<span data-ttu-id="a867b-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="a867b-114">App display name.</span></span> <span data-ttu-id="a867b-115">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a867b-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="a867b-116">description</span><span class="sxs-lookup"><span data-stu-id="a867b-116">description</span></span>|<span data-ttu-id="a867b-117">Строка</span><span class="sxs-lookup"><span data-stu-id="a867b-117">String</span></span>|<span data-ttu-id="a867b-118">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a867b-118">The app's description.</span></span> <span data-ttu-id="a867b-119">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a867b-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="a867b-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="a867b-120">publisherName</span></span>|<span data-ttu-id="a867b-121">String</span><span class="sxs-lookup"><span data-stu-id="a867b-121">String</span></span>|<span data-ttu-id="a867b-122">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a867b-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="a867b-123">productName</span><span class="sxs-lookup"><span data-stu-id="a867b-123">productName</span></span>|<span data-ttu-id="a867b-124">String</span><span class="sxs-lookup"><span data-stu-id="a867b-124">String</span></span>|<span data-ttu-id="a867b-125">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="a867b-125">The product name.</span></span> <span data-ttu-id="a867b-126">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a867b-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="a867b-127">denied</span><span class="sxs-lookup"><span data-stu-id="a867b-127">denied</span></span>|<span data-ttu-id="a867b-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="a867b-128">Boolean</span></span>|<span data-ttu-id="a867b-129">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="a867b-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="a867b-130">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a867b-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="a867b-131">binaryName</span><span class="sxs-lookup"><span data-stu-id="a867b-131">binaryName</span></span>|<span data-ttu-id="a867b-132">String</span><span class="sxs-lookup"><span data-stu-id="a867b-132">String</span></span>|<span data-ttu-id="a867b-133">Двоичное имя.</span><span class="sxs-lookup"><span data-stu-id="a867b-133">The binary name.</span></span>|
|<span data-ttu-id="a867b-134">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="a867b-134">binaryVersionLow</span></span>|<span data-ttu-id="a867b-135">String</span><span class="sxs-lookup"><span data-stu-id="a867b-135">String</span></span>|<span data-ttu-id="a867b-136">Нижняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="a867b-136">The lower binary version.</span></span>|
|<span data-ttu-id="a867b-137">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="a867b-137">binaryVersionHigh</span></span>|<span data-ttu-id="a867b-138">String</span><span class="sxs-lookup"><span data-stu-id="a867b-138">String</span></span>|<span data-ttu-id="a867b-139">Верхняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="a867b-139">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a867b-140">Связи</span><span class="sxs-lookup"><span data-stu-id="a867b-140">Relationships</span></span>
<span data-ttu-id="a867b-141">Нет</span><span class="sxs-lookup"><span data-stu-id="a867b-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a867b-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a867b-142">JSON Representation</span></span>
<span data-ttu-id="a867b-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a867b-143">Here is a JSON representation of the resource.</span></span>
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







