---
title: Тип ресурса windowsInformationProtectionStoreApp
description: Защита данных приложений для Windows из Microsoft Store
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5036a63aff80d3065df7a8e831b0784484dadde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561854"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="606bc-103">Тип ресурса windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="606bc-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="606bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="606bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="606bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="606bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="606bc-106">Защита данных приложений для Windows из Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="606bc-106">Store App for Windows information protection</span></span>


<span data-ttu-id="606bc-107">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="606bc-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="606bc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="606bc-108">Properties</span></span>
|<span data-ttu-id="606bc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="606bc-109">Property</span></span>|<span data-ttu-id="606bc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="606bc-110">Type</span></span>|<span data-ttu-id="606bc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="606bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="606bc-112">displayName</span><span class="sxs-lookup"><span data-stu-id="606bc-112">displayName</span></span>|<span data-ttu-id="606bc-113">Строка</span><span class="sxs-lookup"><span data-stu-id="606bc-113">String</span></span>|<span data-ttu-id="606bc-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="606bc-114">App display name.</span></span> <span data-ttu-id="606bc-115">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="606bc-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="606bc-116">description</span><span class="sxs-lookup"><span data-stu-id="606bc-116">description</span></span>|<span data-ttu-id="606bc-117">String</span><span class="sxs-lookup"><span data-stu-id="606bc-117">String</span></span>|<span data-ttu-id="606bc-118">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="606bc-118">The app's description.</span></span> <span data-ttu-id="606bc-119">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="606bc-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="606bc-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="606bc-120">publisherName</span></span>|<span data-ttu-id="606bc-121">String</span><span class="sxs-lookup"><span data-stu-id="606bc-121">String</span></span>|<span data-ttu-id="606bc-122">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="606bc-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="606bc-123">productName</span><span class="sxs-lookup"><span data-stu-id="606bc-123">productName</span></span>|<span data-ttu-id="606bc-124">String</span><span class="sxs-lookup"><span data-stu-id="606bc-124">String</span></span>|<span data-ttu-id="606bc-125">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="606bc-125">The product name.</span></span> <span data-ttu-id="606bc-126">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="606bc-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="606bc-127">denied</span><span class="sxs-lookup"><span data-stu-id="606bc-127">denied</span></span>|<span data-ttu-id="606bc-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="606bc-128">Boolean</span></span>|<span data-ttu-id="606bc-129">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="606bc-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="606bc-130">Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="606bc-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="606bc-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="606bc-131">Relationships</span></span>
<span data-ttu-id="606bc-132">Нет</span><span class="sxs-lookup"><span data-stu-id="606bc-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="606bc-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="606bc-133">JSON Representation</span></span>
<span data-ttu-id="606bc-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="606bc-134">Here is a JSON representation of the resource.</span></span>
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





