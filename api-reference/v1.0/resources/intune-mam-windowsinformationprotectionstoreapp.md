---
title: Тип ресурса windowsInformationProtectionStoreApp
description: Защита данных приложений для Windows из Microsoft Store
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c15becc47164fd57bbe3d157e9732531a20ebaff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459681"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="c0391-103">Тип ресурса windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="c0391-103">windowsInformationProtectionStoreApp resource type</span></span>

<span data-ttu-id="c0391-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0391-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0391-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0391-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0391-106">Защита данных приложений для Windows из Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="c0391-106">Store App for Windows information protection</span></span>


<span data-ttu-id="c0391-107">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c0391-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0391-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0391-108">Properties</span></span>
|<span data-ttu-id="c0391-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0391-109">Property</span></span>|<span data-ttu-id="c0391-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c0391-110">Type</span></span>|<span data-ttu-id="c0391-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c0391-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0391-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c0391-112">displayName</span></span>|<span data-ttu-id="c0391-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c0391-113">String</span></span>|<span data-ttu-id="c0391-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="c0391-114">App display name.</span></span> <span data-ttu-id="c0391-115">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c0391-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c0391-116">description</span><span class="sxs-lookup"><span data-stu-id="c0391-116">description</span></span>|<span data-ttu-id="c0391-117">Строка</span><span class="sxs-lookup"><span data-stu-id="c0391-117">String</span></span>|<span data-ttu-id="c0391-118">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c0391-118">The app's description.</span></span> <span data-ttu-id="c0391-119">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c0391-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c0391-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="c0391-120">publisherName</span></span>|<span data-ttu-id="c0391-121">String</span><span class="sxs-lookup"><span data-stu-id="c0391-121">String</span></span>|<span data-ttu-id="c0391-122">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c0391-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c0391-123">productName</span><span class="sxs-lookup"><span data-stu-id="c0391-123">productName</span></span>|<span data-ttu-id="c0391-124">String</span><span class="sxs-lookup"><span data-stu-id="c0391-124">String</span></span>|<span data-ttu-id="c0391-125">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="c0391-125">The product name.</span></span> <span data-ttu-id="c0391-126">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c0391-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="c0391-127">denied</span><span class="sxs-lookup"><span data-stu-id="c0391-127">denied</span></span>|<span data-ttu-id="c0391-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0391-128">Boolean</span></span>|<span data-ttu-id="c0391-129">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="c0391-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="c0391-130">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c0391-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0391-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="c0391-131">Relationships</span></span>
<span data-ttu-id="c0391-132">Нет</span><span class="sxs-lookup"><span data-stu-id="c0391-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0391-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0391-133">JSON Representation</span></span>
<span data-ttu-id="c0391-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0391-134">Here is a JSON representation of the resource.</span></span>
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







