---
title: Тип ресурса windowsInformationProtectionDesktopApp
description: Защита данных классических приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba45dd4f3bb450cfc9822fb68f1b4511f69da2fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977390"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="b3761-103">Тип ресурса windowsInformationProtectionDesktopApp</span><span class="sxs-lookup"><span data-stu-id="b3761-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="b3761-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b3761-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3761-105">Защита данных классических приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="b3761-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="b3761-106">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3761-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3761-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3761-107">Properties</span></span>
|<span data-ttu-id="b3761-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3761-108">Property</span></span>|<span data-ttu-id="b3761-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b3761-109">Type</span></span>|<span data-ttu-id="b3761-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b3761-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3761-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b3761-111">displayName</span></span>|<span data-ttu-id="b3761-112">String</span><span class="sxs-lookup"><span data-stu-id="b3761-112">String</span></span>|<span data-ttu-id="b3761-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="b3761-113">App display name.</span></span> <span data-ttu-id="b3761-114">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3761-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b3761-115">описание</span><span class="sxs-lookup"><span data-stu-id="b3761-115">description</span></span>|<span data-ttu-id="b3761-116">String</span><span class="sxs-lookup"><span data-stu-id="b3761-116">String</span></span>|<span data-ttu-id="b3761-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b3761-117">The app's description.</span></span> <span data-ttu-id="b3761-118">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3761-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b3761-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="b3761-119">publisherName</span></span>|<span data-ttu-id="b3761-120">String</span><span class="sxs-lookup"><span data-stu-id="b3761-120">String</span></span>|<span data-ttu-id="b3761-121">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3761-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b3761-122">productName</span><span class="sxs-lookup"><span data-stu-id="b3761-122">productName</span></span>|<span data-ttu-id="b3761-123">String</span><span class="sxs-lookup"><span data-stu-id="b3761-123">String</span></span>|<span data-ttu-id="b3761-124">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="b3761-124">The product name.</span></span> <span data-ttu-id="b3761-125">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3761-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b3761-126">denied</span><span class="sxs-lookup"><span data-stu-id="b3761-126">denied</span></span>|<span data-ttu-id="b3761-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3761-127">Boolean</span></span>|<span data-ttu-id="b3761-128">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="b3761-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="b3761-129">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b3761-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b3761-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="b3761-130">binaryName</span></span>|<span data-ttu-id="b3761-131">String</span><span class="sxs-lookup"><span data-stu-id="b3761-131">String</span></span>|<span data-ttu-id="b3761-132">Двоичное имя.</span><span class="sxs-lookup"><span data-stu-id="b3761-132">The binary name.</span></span>|
|<span data-ttu-id="b3761-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="b3761-133">binaryVersionLow</span></span>|<span data-ttu-id="b3761-134">String</span><span class="sxs-lookup"><span data-stu-id="b3761-134">String</span></span>|<span data-ttu-id="b3761-135">Нижняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="b3761-135">The lower binary version.</span></span>|
|<span data-ttu-id="b3761-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="b3761-136">binaryVersionHigh</span></span>|<span data-ttu-id="b3761-137">String</span><span class="sxs-lookup"><span data-stu-id="b3761-137">String</span></span>|<span data-ttu-id="b3761-138">Верхняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="b3761-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3761-139">Связи</span><span class="sxs-lookup"><span data-stu-id="b3761-139">Relationships</span></span>
<span data-ttu-id="b3761-140">Нет</span><span class="sxs-lookup"><span data-stu-id="b3761-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3761-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3761-141">JSON Representation</span></span>
<span data-ttu-id="b3761-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3761-142">Here is a JSON representation of the resource.</span></span>
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



