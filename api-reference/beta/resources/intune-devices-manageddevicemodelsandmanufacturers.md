---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7cfedad0fce093d8fc3358afcf622ac8beb58d6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999776"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="60820-103">Тип ресурса Манажеддевицемоделсандмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="60820-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="60820-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60820-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60820-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60820-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60820-106">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="60820-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="60820-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="60820-107">Properties</span></span>
|<span data-ttu-id="60820-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="60820-108">Property</span></span>|<span data-ttu-id="60820-109">Тип</span><span class="sxs-lookup"><span data-stu-id="60820-109">Type</span></span>|<span data-ttu-id="60820-110">Описание</span><span class="sxs-lookup"><span data-stu-id="60820-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60820-111">Девицемоделс</span><span class="sxs-lookup"><span data-stu-id="60820-111">deviceModels</span></span>|<span data-ttu-id="60820-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="60820-112">String collection</span></span>|<span data-ttu-id="60820-113">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="60820-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="60820-114">Девицемануфактурерс</span><span class="sxs-lookup"><span data-stu-id="60820-114">deviceManufacturers</span></span>|<span data-ttu-id="60820-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="60820-115">String collection</span></span>|<span data-ttu-id="60820-116">Список производства для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="60820-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="60820-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="60820-117">Relationships</span></span>
<span data-ttu-id="60820-118">Нет</span><span class="sxs-lookup"><span data-stu-id="60820-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60820-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60820-119">JSON Representation</span></span>
<span data-ttu-id="60820-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60820-120">Here is a JSON representation of the resource.</span></span>
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





