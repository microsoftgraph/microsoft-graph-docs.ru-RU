---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4a64b1b91df7bc52fbec718e0bc5fb13beae308
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468483"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="5385a-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="5385a-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="5385a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5385a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5385a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5385a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5385a-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="5385a-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="5385a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5385a-107">Properties</span></span>
|<span data-ttu-id="5385a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5385a-108">Property</span></span>|<span data-ttu-id="5385a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5385a-109">Type</span></span>|<span data-ttu-id="5385a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5385a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5385a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5385a-111">displayName</span></span>|<span data-ttu-id="5385a-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5385a-112">String</span></span>|<span data-ttu-id="5385a-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="5385a-113">App display name.</span></span>|
|<span data-ttu-id="5385a-114">description</span><span class="sxs-lookup"><span data-stu-id="5385a-114">description</span></span>|<span data-ttu-id="5385a-115">Строка</span><span class="sxs-lookup"><span data-stu-id="5385a-115">String</span></span>|<span data-ttu-id="5385a-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5385a-116">The app's description.</span></span>|
|<span data-ttu-id="5385a-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="5385a-117">publisherName</span></span>|<span data-ttu-id="5385a-118">String</span><span class="sxs-lookup"><span data-stu-id="5385a-118">String</span></span>|<span data-ttu-id="5385a-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="5385a-119">The publisher name</span></span>|
|<span data-ttu-id="5385a-120">productName</span><span class="sxs-lookup"><span data-stu-id="5385a-120">productName</span></span>|<span data-ttu-id="5385a-121">String</span><span class="sxs-lookup"><span data-stu-id="5385a-121">String</span></span>|<span data-ttu-id="5385a-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="5385a-122">The product name.</span></span>|
|<span data-ttu-id="5385a-123">denied</span><span class="sxs-lookup"><span data-stu-id="5385a-123">denied</span></span>|<span data-ttu-id="5385a-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5385a-124">Boolean</span></span>|<span data-ttu-id="5385a-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="5385a-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5385a-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="5385a-126">Relationships</span></span>
<span data-ttu-id="5385a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="5385a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5385a-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5385a-128">JSON Representation</span></span>
<span data-ttu-id="5385a-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5385a-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```







