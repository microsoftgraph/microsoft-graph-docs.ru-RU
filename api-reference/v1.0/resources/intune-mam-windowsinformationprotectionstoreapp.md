---
title: Тип ресурса windowsInformationProtectionStoreApp
description: Защита данных приложений для Windows из Microsoft Store
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dafad17c55ebd045dcb2c588c005cb94efb21edc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448181"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="0e091-103">Тип ресурса windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="0e091-103">windowsInformationProtectionStoreApp resource type</span></span>

<span data-ttu-id="0e091-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0e091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e091-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e091-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e091-106">Защита данных приложений для Windows из Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="0e091-106">Store App for Windows information protection</span></span>


<span data-ttu-id="0e091-107">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0e091-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0e091-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e091-108">Properties</span></span>
|<span data-ttu-id="0e091-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e091-109">Property</span></span>|<span data-ttu-id="0e091-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0e091-110">Type</span></span>|<span data-ttu-id="0e091-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0e091-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e091-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0e091-112">displayName</span></span>|<span data-ttu-id="0e091-113">Строка</span><span class="sxs-lookup"><span data-stu-id="0e091-113">String</span></span>|<span data-ttu-id="0e091-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="0e091-114">App display name.</span></span> <span data-ttu-id="0e091-115">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0e091-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0e091-116">description</span><span class="sxs-lookup"><span data-stu-id="0e091-116">description</span></span>|<span data-ttu-id="0e091-117">Строка</span><span class="sxs-lookup"><span data-stu-id="0e091-117">String</span></span>|<span data-ttu-id="0e091-118">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0e091-118">The app's description.</span></span> <span data-ttu-id="0e091-119">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0e091-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0e091-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="0e091-120">publisherName</span></span>|<span data-ttu-id="0e091-121">String</span><span class="sxs-lookup"><span data-stu-id="0e091-121">String</span></span>|<span data-ttu-id="0e091-122">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0e091-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0e091-123">productName</span><span class="sxs-lookup"><span data-stu-id="0e091-123">productName</span></span>|<span data-ttu-id="0e091-124">String</span><span class="sxs-lookup"><span data-stu-id="0e091-124">String</span></span>|<span data-ttu-id="0e091-125">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="0e091-125">The product name.</span></span> <span data-ttu-id="0e091-126">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0e091-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0e091-127">denied</span><span class="sxs-lookup"><span data-stu-id="0e091-127">denied</span></span>|<span data-ttu-id="0e091-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e091-128">Boolean</span></span>|<span data-ttu-id="0e091-129">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="0e091-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="0e091-130">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0e091-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e091-131">Связи</span><span class="sxs-lookup"><span data-stu-id="0e091-131">Relationships</span></span>
<span data-ttu-id="0e091-132">Нет</span><span class="sxs-lookup"><span data-stu-id="0e091-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e091-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e091-133">JSON Representation</span></span>
<span data-ttu-id="0e091-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e091-134">Here is a JSON representation of the resource.</span></span>
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




