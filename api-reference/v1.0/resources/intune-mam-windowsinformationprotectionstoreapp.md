---
title: Тип ресурса windowsInformationProtectionStoreApp
description: Защита данных приложений для Windows из Microsoft Store
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e67e76dcec3390f172f4d2819bf7d22ee63f7da5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262547"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="61f68-103">Тип ресурса windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="61f68-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="61f68-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61f68-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61f68-105">Защита данных приложений для Windows из Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="61f68-105">Store App for Windows information protection</span></span>


<span data-ttu-id="61f68-106">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f68-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="61f68-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="61f68-107">Properties</span></span>
|<span data-ttu-id="61f68-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="61f68-108">Property</span></span>|<span data-ttu-id="61f68-109">Тип</span><span class="sxs-lookup"><span data-stu-id="61f68-109">Type</span></span>|<span data-ttu-id="61f68-110">Описание</span><span class="sxs-lookup"><span data-stu-id="61f68-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61f68-111">displayName</span><span class="sxs-lookup"><span data-stu-id="61f68-111">displayName</span></span>|<span data-ttu-id="61f68-112">String</span><span class="sxs-lookup"><span data-stu-id="61f68-112">String</span></span>|<span data-ttu-id="61f68-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="61f68-113">App display name.</span></span> <span data-ttu-id="61f68-114">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f68-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="61f68-115">description</span><span class="sxs-lookup"><span data-stu-id="61f68-115">description</span></span>|<span data-ttu-id="61f68-116">Строка</span><span class="sxs-lookup"><span data-stu-id="61f68-116">String</span></span>|<span data-ttu-id="61f68-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="61f68-117">The app's description.</span></span> <span data-ttu-id="61f68-118">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f68-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="61f68-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="61f68-119">publisherName</span></span>|<span data-ttu-id="61f68-120">String</span><span class="sxs-lookup"><span data-stu-id="61f68-120">String</span></span>|<span data-ttu-id="61f68-121">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f68-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="61f68-122">productName</span><span class="sxs-lookup"><span data-stu-id="61f68-122">productName</span></span>|<span data-ttu-id="61f68-123">String</span><span class="sxs-lookup"><span data-stu-id="61f68-123">String</span></span>|<span data-ttu-id="61f68-124">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="61f68-124">The product name.</span></span> <span data-ttu-id="61f68-125">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f68-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="61f68-126">denied</span><span class="sxs-lookup"><span data-stu-id="61f68-126">denied</span></span>|<span data-ttu-id="61f68-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="61f68-127">Boolean</span></span>|<span data-ttu-id="61f68-128">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="61f68-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="61f68-129">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f68-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="61f68-130">Связи</span><span class="sxs-lookup"><span data-stu-id="61f68-130">Relationships</span></span>
<span data-ttu-id="61f68-131">Нет</span><span class="sxs-lookup"><span data-stu-id="61f68-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61f68-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61f68-132">JSON Representation</span></span>
<span data-ttu-id="61f68-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61f68-133">Here is a JSON representation of the resource.</span></span>
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



