---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 32dd1213bb06fbaa80a744d78453b12f6eeff7dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037760"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="56569-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="56569-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="56569-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56569-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56569-105">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="56569-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="56569-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="56569-106">Properties</span></span>
|<span data-ttu-id="56569-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="56569-107">Property</span></span>|<span data-ttu-id="56569-108">Тип</span><span class="sxs-lookup"><span data-stu-id="56569-108">Type</span></span>|<span data-ttu-id="56569-109">Описание</span><span class="sxs-lookup"><span data-stu-id="56569-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56569-110">displayName</span><span class="sxs-lookup"><span data-stu-id="56569-110">displayName</span></span>|<span data-ttu-id="56569-111">Строка</span><span class="sxs-lookup"><span data-stu-id="56569-111">String</span></span>|<span data-ttu-id="56569-112">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="56569-112">App display name.</span></span>|
|<span data-ttu-id="56569-113">description</span><span class="sxs-lookup"><span data-stu-id="56569-113">description</span></span>|<span data-ttu-id="56569-114">Строка</span><span class="sxs-lookup"><span data-stu-id="56569-114">String</span></span>|<span data-ttu-id="56569-115">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="56569-115">The app's description.</span></span>|
|<span data-ttu-id="56569-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="56569-116">publisherName</span></span>|<span data-ttu-id="56569-117">String</span><span class="sxs-lookup"><span data-stu-id="56569-117">String</span></span>|<span data-ttu-id="56569-118">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="56569-118">The publisher name</span></span>|
|<span data-ttu-id="56569-119">productName</span><span class="sxs-lookup"><span data-stu-id="56569-119">productName</span></span>|<span data-ttu-id="56569-120">String</span><span class="sxs-lookup"><span data-stu-id="56569-120">String</span></span>|<span data-ttu-id="56569-121">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="56569-121">The product name.</span></span>|
|<span data-ttu-id="56569-122">denied</span><span class="sxs-lookup"><span data-stu-id="56569-122">denied</span></span>|<span data-ttu-id="56569-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="56569-123">Boolean</span></span>|<span data-ttu-id="56569-124">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="56569-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56569-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="56569-125">Relationships</span></span>
<span data-ttu-id="56569-126">Нет</span><span class="sxs-lookup"><span data-stu-id="56569-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56569-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56569-127">JSON Representation</span></span>
<span data-ttu-id="56569-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56569-128">Here is a JSON representation of the resource.</span></span>
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



