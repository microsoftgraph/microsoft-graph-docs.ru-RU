---
title: Тип ресурса windowsInformationProtectionStoreApp
description: Защита данных приложений для Windows из Microsoft Store
author: tfitzmac
ms.openlocfilehash: b5f13b77a5fbd9464ac968034fb19ae4e6327b9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344669"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="df825-103">Тип ресурса windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="df825-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="df825-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="df825-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df825-105">Защита данных приложений для Windows из Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="df825-105">Store App for Windows information protection</span></span>

<span data-ttu-id="df825-106">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="df825-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df825-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="df825-107">Properties</span></span>
|<span data-ttu-id="df825-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="df825-108">Property</span></span>|<span data-ttu-id="df825-109">Тип</span><span class="sxs-lookup"><span data-stu-id="df825-109">Type</span></span>|<span data-ttu-id="df825-110">Описание</span><span class="sxs-lookup"><span data-stu-id="df825-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df825-111">displayName</span><span class="sxs-lookup"><span data-stu-id="df825-111">displayName</span></span>|<span data-ttu-id="df825-112">String</span><span class="sxs-lookup"><span data-stu-id="df825-112">String</span></span>|<span data-ttu-id="df825-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="df825-113">App display name.</span></span> <span data-ttu-id="df825-114">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="df825-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="df825-115">описание</span><span class="sxs-lookup"><span data-stu-id="df825-115">description</span></span>|<span data-ttu-id="df825-116">String</span><span class="sxs-lookup"><span data-stu-id="df825-116">String</span></span>|<span data-ttu-id="df825-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="df825-117">The app's description.</span></span> <span data-ttu-id="df825-118">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="df825-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="df825-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="df825-119">publisherName</span></span>|<span data-ttu-id="df825-120">String</span><span class="sxs-lookup"><span data-stu-id="df825-120">String</span></span>|<span data-ttu-id="df825-121">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="df825-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="df825-122">productName</span><span class="sxs-lookup"><span data-stu-id="df825-122">productName</span></span>|<span data-ttu-id="df825-123">String</span><span class="sxs-lookup"><span data-stu-id="df825-123">String</span></span>|<span data-ttu-id="df825-124">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="df825-124">The product name.</span></span> <span data-ttu-id="df825-125">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="df825-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="df825-126">denied</span><span class="sxs-lookup"><span data-stu-id="df825-126">denied</span></span>|<span data-ttu-id="df825-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="df825-127">Boolean</span></span>|<span data-ttu-id="df825-128">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="df825-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="df825-129">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="df825-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="df825-130">Связи</span><span class="sxs-lookup"><span data-stu-id="df825-130">Relationships</span></span>
<span data-ttu-id="df825-131">Нет</span><span class="sxs-lookup"><span data-stu-id="df825-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df825-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df825-132">JSON Representation</span></span>
<span data-ttu-id="df825-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df825-133">Here is a JSON representation of the resource.</span></span>
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



