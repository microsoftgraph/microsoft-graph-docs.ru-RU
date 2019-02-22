---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2b8739fd045d4b8e6293164fc7e9b14154a475c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139286"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="1f08e-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="1f08e-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="1f08e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f08e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f08e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f08e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f08e-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="1f08e-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="1f08e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f08e-107">Properties</span></span>
|<span data-ttu-id="1f08e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f08e-108">Property</span></span>|<span data-ttu-id="1f08e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1f08e-109">Type</span></span>|<span data-ttu-id="1f08e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f08e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f08e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1f08e-111">displayName</span></span>|<span data-ttu-id="1f08e-112">String</span><span class="sxs-lookup"><span data-stu-id="1f08e-112">String</span></span>|<span data-ttu-id="1f08e-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="1f08e-113">App display name.</span></span>|
|<span data-ttu-id="1f08e-114">description</span><span class="sxs-lookup"><span data-stu-id="1f08e-114">description</span></span>|<span data-ttu-id="1f08e-115">Строка</span><span class="sxs-lookup"><span data-stu-id="1f08e-115">String</span></span>|<span data-ttu-id="1f08e-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1f08e-116">The app's description.</span></span>|
|<span data-ttu-id="1f08e-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="1f08e-117">publisherName</span></span>|<span data-ttu-id="1f08e-118">String</span><span class="sxs-lookup"><span data-stu-id="1f08e-118">String</span></span>|<span data-ttu-id="1f08e-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="1f08e-119">The publisher name</span></span>|
|<span data-ttu-id="1f08e-120">productName</span><span class="sxs-lookup"><span data-stu-id="1f08e-120">productName</span></span>|<span data-ttu-id="1f08e-121">String</span><span class="sxs-lookup"><span data-stu-id="1f08e-121">String</span></span>|<span data-ttu-id="1f08e-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="1f08e-122">The product name.</span></span>|
|<span data-ttu-id="1f08e-123">denied</span><span class="sxs-lookup"><span data-stu-id="1f08e-123">denied</span></span>|<span data-ttu-id="1f08e-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f08e-124">Boolean</span></span>|<span data-ttu-id="1f08e-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="1f08e-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f08e-126">Связи</span><span class="sxs-lookup"><span data-stu-id="1f08e-126">Relationships</span></span>
<span data-ttu-id="1f08e-127">Нет</span><span class="sxs-lookup"><span data-stu-id="1f08e-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f08e-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f08e-128">JSON Representation</span></span>
<span data-ttu-id="1f08e-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f08e-129">Here is a JSON representation of the resource.</span></span>
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




