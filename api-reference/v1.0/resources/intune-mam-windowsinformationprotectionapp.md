---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f3a53ffd35ced4b40476868e7e492364ec8ffa0d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367352"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="7bc76-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="7bc76-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="7bc76-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bc76-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bc76-105">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="7bc76-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="7bc76-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bc76-106">Properties</span></span>
|<span data-ttu-id="7bc76-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bc76-107">Property</span></span>|<span data-ttu-id="7bc76-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7bc76-108">Type</span></span>|<span data-ttu-id="7bc76-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7bc76-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bc76-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7bc76-110">displayName</span></span>|<span data-ttu-id="7bc76-111">Строка</span><span class="sxs-lookup"><span data-stu-id="7bc76-111">String</span></span>|<span data-ttu-id="7bc76-112">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc76-112">App display name.</span></span>|
|<span data-ttu-id="7bc76-113">description</span><span class="sxs-lookup"><span data-stu-id="7bc76-113">description</span></span>|<span data-ttu-id="7bc76-114">Строка</span><span class="sxs-lookup"><span data-stu-id="7bc76-114">String</span></span>|<span data-ttu-id="7bc76-115">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc76-115">The app's description.</span></span>|
|<span data-ttu-id="7bc76-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="7bc76-116">publisherName</span></span>|<span data-ttu-id="7bc76-117">String</span><span class="sxs-lookup"><span data-stu-id="7bc76-117">String</span></span>|<span data-ttu-id="7bc76-118">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="7bc76-118">The publisher name</span></span>|
|<span data-ttu-id="7bc76-119">productName</span><span class="sxs-lookup"><span data-stu-id="7bc76-119">productName</span></span>|<span data-ttu-id="7bc76-120">String</span><span class="sxs-lookup"><span data-stu-id="7bc76-120">String</span></span>|<span data-ttu-id="7bc76-121">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="7bc76-121">The product name.</span></span>|
|<span data-ttu-id="7bc76-122">denied</span><span class="sxs-lookup"><span data-stu-id="7bc76-122">denied</span></span>|<span data-ttu-id="7bc76-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="7bc76-123">Boolean</span></span>|<span data-ttu-id="7bc76-124">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="7bc76-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bc76-125">Связи</span><span class="sxs-lookup"><span data-stu-id="7bc76-125">Relationships</span></span>
<span data-ttu-id="7bc76-126">Нет</span><span class="sxs-lookup"><span data-stu-id="7bc76-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bc76-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bc76-127">JSON Representation</span></span>
<span data-ttu-id="7bc76-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bc76-128">Here is a JSON representation of the resource.</span></span>
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




