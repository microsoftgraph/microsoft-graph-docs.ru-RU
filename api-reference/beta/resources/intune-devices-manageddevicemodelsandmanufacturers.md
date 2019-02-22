---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfd8f068305bdae86a0acc9ef5f9113bb0d1c579
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148302"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="79f39-103">Тип ресурса Манажеддевицемоделсандмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="79f39-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="79f39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79f39-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79f39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79f39-106">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="79f39-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="79f39-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="79f39-107">Properties</span></span>
|<span data-ttu-id="79f39-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="79f39-108">Property</span></span>|<span data-ttu-id="79f39-109">Тип</span><span class="sxs-lookup"><span data-stu-id="79f39-109">Type</span></span>|<span data-ttu-id="79f39-110">Описание</span><span class="sxs-lookup"><span data-stu-id="79f39-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79f39-111">Девицемоделс</span><span class="sxs-lookup"><span data-stu-id="79f39-111">deviceModels</span></span>|<span data-ttu-id="79f39-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="79f39-112">String collection</span></span>|<span data-ttu-id="79f39-113">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="79f39-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="79f39-114">Девицемануфактурерс</span><span class="sxs-lookup"><span data-stu-id="79f39-114">deviceManufacturers</span></span>|<span data-ttu-id="79f39-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="79f39-115">String collection</span></span>|<span data-ttu-id="79f39-116">Список производства для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="79f39-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="79f39-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="79f39-117">Relationships</span></span>
<span data-ttu-id="79f39-118">Нет</span><span class="sxs-lookup"><span data-stu-id="79f39-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79f39-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79f39-119">JSON Representation</span></span>
<span data-ttu-id="79f39-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79f39-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```




