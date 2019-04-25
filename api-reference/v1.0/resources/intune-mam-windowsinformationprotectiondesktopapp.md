---
title: Тип ресурса windowsInformationProtectionDesktopApp
description: Защита данных классических приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83ad9e3e500ab5276e4643055f602e763de34fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564255"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="c5137-103">Тип ресурса windowsInformationProtectionDesktopApp</span><span class="sxs-lookup"><span data-stu-id="c5137-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="c5137-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5137-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5137-105">Защита данных классических приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="c5137-105">Desktop App for Windows information protection</span></span>


<span data-ttu-id="c5137-106">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5137-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5137-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5137-107">Properties</span></span>
|<span data-ttu-id="c5137-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5137-108">Property</span></span>|<span data-ttu-id="c5137-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c5137-109">Type</span></span>|<span data-ttu-id="c5137-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5137-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5137-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c5137-111">displayName</span></span>|<span data-ttu-id="c5137-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c5137-112">String</span></span>|<span data-ttu-id="c5137-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="c5137-113">App display name.</span></span> <span data-ttu-id="c5137-114">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5137-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c5137-115">description</span><span class="sxs-lookup"><span data-stu-id="c5137-115">description</span></span>|<span data-ttu-id="c5137-116">String</span><span class="sxs-lookup"><span data-stu-id="c5137-116">String</span></span>|<span data-ttu-id="c5137-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c5137-117">The app's description.</span></span> <span data-ttu-id="c5137-118">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5137-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c5137-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="c5137-119">publisherName</span></span>|<span data-ttu-id="c5137-120">String</span><span class="sxs-lookup"><span data-stu-id="c5137-120">String</span></span>|<span data-ttu-id="c5137-121">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5137-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c5137-122">productName</span><span class="sxs-lookup"><span data-stu-id="c5137-122">productName</span></span>|<span data-ttu-id="c5137-123">String</span><span class="sxs-lookup"><span data-stu-id="c5137-123">String</span></span>|<span data-ttu-id="c5137-124">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="c5137-124">The product name.</span></span> <span data-ttu-id="c5137-125">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5137-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c5137-126">denied</span><span class="sxs-lookup"><span data-stu-id="c5137-126">denied</span></span>|<span data-ttu-id="c5137-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5137-127">Boolean</span></span>|<span data-ttu-id="c5137-128">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="c5137-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="c5137-129">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5137-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c5137-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="c5137-130">binaryName</span></span>|<span data-ttu-id="c5137-131">String</span><span class="sxs-lookup"><span data-stu-id="c5137-131">String</span></span>|<span data-ttu-id="c5137-132">Двоичное имя.</span><span class="sxs-lookup"><span data-stu-id="c5137-132">The binary name.</span></span>|
|<span data-ttu-id="c5137-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="c5137-133">binaryVersionLow</span></span>|<span data-ttu-id="c5137-134">String</span><span class="sxs-lookup"><span data-stu-id="c5137-134">String</span></span>|<span data-ttu-id="c5137-135">Нижняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="c5137-135">The lower binary version.</span></span>|
|<span data-ttu-id="c5137-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="c5137-136">binaryVersionHigh</span></span>|<span data-ttu-id="c5137-137">String</span><span class="sxs-lookup"><span data-stu-id="c5137-137">String</span></span>|<span data-ttu-id="c5137-138">Верхняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="c5137-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5137-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="c5137-139">Relationships</span></span>
<span data-ttu-id="c5137-140">Нет</span><span class="sxs-lookup"><span data-stu-id="c5137-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5137-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5137-141">JSON Representation</span></span>
<span data-ttu-id="c5137-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5137-142">Here is a JSON representation of the resource.</span></span>
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



