---
title: тип ресурса chromeOSDeviceProperty
description: Представляет свойство устройства ChromeOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42b4903965d90641955659277360c46428562ed4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667010"
---
# <a name="chromeosdeviceproperty-resource-type"></a><span data-ttu-id="a676e-103">тип ресурса chromeOSDeviceProperty</span><span class="sxs-lookup"><span data-stu-id="a676e-103">chromeOSDeviceProperty resource type</span></span>

<span data-ttu-id="a676e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a676e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a676e-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a676e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a676e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a676e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a676e-107">Представляет свойство устройства ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="a676e-107">Represents a property of the ChromeOS device.</span></span>

## <a name="properties"></a><span data-ttu-id="a676e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a676e-108">Properties</span></span>
|<span data-ttu-id="a676e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a676e-109">Property</span></span>|<span data-ttu-id="a676e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a676e-110">Type</span></span>|<span data-ttu-id="a676e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a676e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a676e-112">name</span><span class="sxs-lookup"><span data-stu-id="a676e-112">name</span></span>|<span data-ttu-id="a676e-113">String</span><span class="sxs-lookup"><span data-stu-id="a676e-113">String</span></span>|<span data-ttu-id="a676e-114">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a676e-114">Name of the property</span></span>|
|<span data-ttu-id="a676e-115">value</span><span class="sxs-lookup"><span data-stu-id="a676e-115">value</span></span>|<span data-ttu-id="a676e-116">String</span><span class="sxs-lookup"><span data-stu-id="a676e-116">String</span></span>|<span data-ttu-id="a676e-117">Значение свойства</span><span class="sxs-lookup"><span data-stu-id="a676e-117">Value of the property</span></span>|
|<span data-ttu-id="a676e-118">valueType</span><span class="sxs-lookup"><span data-stu-id="a676e-118">valueType</span></span>|<span data-ttu-id="a676e-119">Строка</span><span class="sxs-lookup"><span data-stu-id="a676e-119">String</span></span>|<span data-ttu-id="a676e-120">Тип значения</span><span class="sxs-lookup"><span data-stu-id="a676e-120">Type of the value</span></span>|
|<span data-ttu-id="a676e-121">updatable</span><span class="sxs-lookup"><span data-stu-id="a676e-121">updatable</span></span>|<span data-ttu-id="a676e-122">Логический</span><span class="sxs-lookup"><span data-stu-id="a676e-122">Boolean</span></span>|<span data-ttu-id="a676e-123">Является ли это свойство updatable</span><span class="sxs-lookup"><span data-stu-id="a676e-123">Whether this property is updatable</span></span>|

## <a name="relationships"></a><span data-ttu-id="a676e-124">Связи</span><span class="sxs-lookup"><span data-stu-id="a676e-124">Relationships</span></span>
<span data-ttu-id="a676e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a676e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a676e-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a676e-126">JSON Representation</span></span>
<span data-ttu-id="a676e-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a676e-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chromeOSDeviceProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSDeviceProperty",
  "name": "String",
  "value": "String",
  "valueType": "String",
  "updatable": true
}
```




