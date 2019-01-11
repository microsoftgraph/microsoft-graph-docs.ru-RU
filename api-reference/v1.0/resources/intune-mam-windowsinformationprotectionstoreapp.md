---
title: Тип ресурса windowsInformationProtectionStoreApp
description: Защита данных приложений для Windows из Microsoft Store
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4e78aa854b15763cade9a4d6020f1737bbca1642
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814478"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="098ff-103">Тип ресурса windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="098ff-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="098ff-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="098ff-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="098ff-105">Защита данных приложений для Windows из Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="098ff-105">Store App for Windows information protection</span></span>

<span data-ttu-id="098ff-106">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="098ff-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="098ff-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="098ff-107">Properties</span></span>
|<span data-ttu-id="098ff-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="098ff-108">Property</span></span>|<span data-ttu-id="098ff-109">Тип</span><span class="sxs-lookup"><span data-stu-id="098ff-109">Type</span></span>|<span data-ttu-id="098ff-110">Описание</span><span class="sxs-lookup"><span data-stu-id="098ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="098ff-111">displayName</span><span class="sxs-lookup"><span data-stu-id="098ff-111">displayName</span></span>|<span data-ttu-id="098ff-112">String</span><span class="sxs-lookup"><span data-stu-id="098ff-112">String</span></span>|<span data-ttu-id="098ff-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="098ff-113">App display name.</span></span> <span data-ttu-id="098ff-114">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="098ff-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="098ff-115">описание</span><span class="sxs-lookup"><span data-stu-id="098ff-115">description</span></span>|<span data-ttu-id="098ff-116">String</span><span class="sxs-lookup"><span data-stu-id="098ff-116">String</span></span>|<span data-ttu-id="098ff-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="098ff-117">The app's description.</span></span> <span data-ttu-id="098ff-118">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="098ff-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="098ff-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="098ff-119">publisherName</span></span>|<span data-ttu-id="098ff-120">String</span><span class="sxs-lookup"><span data-stu-id="098ff-120">String</span></span>|<span data-ttu-id="098ff-121">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="098ff-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="098ff-122">productName</span><span class="sxs-lookup"><span data-stu-id="098ff-122">productName</span></span>|<span data-ttu-id="098ff-123">String</span><span class="sxs-lookup"><span data-stu-id="098ff-123">String</span></span>|<span data-ttu-id="098ff-124">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="098ff-124">The product name.</span></span> <span data-ttu-id="098ff-125">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="098ff-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="098ff-126">denied</span><span class="sxs-lookup"><span data-stu-id="098ff-126">denied</span></span>|<span data-ttu-id="098ff-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="098ff-127">Boolean</span></span>|<span data-ttu-id="098ff-128">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="098ff-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="098ff-129">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="098ff-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="098ff-130">Связи</span><span class="sxs-lookup"><span data-stu-id="098ff-130">Relationships</span></span>
<span data-ttu-id="098ff-131">Нет</span><span class="sxs-lookup"><span data-stu-id="098ff-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="098ff-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="098ff-132">JSON Representation</span></span>
<span data-ttu-id="098ff-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="098ff-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



