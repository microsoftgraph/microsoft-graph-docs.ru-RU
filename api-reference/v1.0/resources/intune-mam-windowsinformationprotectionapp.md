---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561204"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="add9e-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="add9e-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="add9e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="add9e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="add9e-105">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="add9e-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="add9e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="add9e-106">Properties</span></span>
|<span data-ttu-id="add9e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="add9e-107">Property</span></span>|<span data-ttu-id="add9e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="add9e-108">Type</span></span>|<span data-ttu-id="add9e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="add9e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="add9e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="add9e-110">displayName</span></span>|<span data-ttu-id="add9e-111">Строка</span><span class="sxs-lookup"><span data-stu-id="add9e-111">String</span></span>|<span data-ttu-id="add9e-112">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="add9e-112">App display name.</span></span>|
|<span data-ttu-id="add9e-113">description</span><span class="sxs-lookup"><span data-stu-id="add9e-113">description</span></span>|<span data-ttu-id="add9e-114">String</span><span class="sxs-lookup"><span data-stu-id="add9e-114">String</span></span>|<span data-ttu-id="add9e-115">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="add9e-115">The app's description.</span></span>|
|<span data-ttu-id="add9e-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="add9e-116">publisherName</span></span>|<span data-ttu-id="add9e-117">String</span><span class="sxs-lookup"><span data-stu-id="add9e-117">String</span></span>|<span data-ttu-id="add9e-118">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="add9e-118">The publisher name</span></span>|
|<span data-ttu-id="add9e-119">productName</span><span class="sxs-lookup"><span data-stu-id="add9e-119">productName</span></span>|<span data-ttu-id="add9e-120">String</span><span class="sxs-lookup"><span data-stu-id="add9e-120">String</span></span>|<span data-ttu-id="add9e-121">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="add9e-121">The product name.</span></span>|
|<span data-ttu-id="add9e-122">denied</span><span class="sxs-lookup"><span data-stu-id="add9e-122">denied</span></span>|<span data-ttu-id="add9e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="add9e-123">Boolean</span></span>|<span data-ttu-id="add9e-124">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="add9e-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="add9e-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="add9e-125">Relationships</span></span>
<span data-ttu-id="add9e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="add9e-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="add9e-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="add9e-127">JSON Representation</span></span>
<span data-ttu-id="add9e-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="add9e-128">Here is a JSON representation of the resource.</span></span>
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



