---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e9846b9d551b7ae226fe13c32100c8cbfd049ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372267"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="a787b-103">Тип ресурса Манажеддевицемоделсандмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="a787b-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="a787b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a787b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a787b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a787b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a787b-106">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="a787b-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="a787b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a787b-107">Properties</span></span>
|<span data-ttu-id="a787b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a787b-108">Property</span></span>|<span data-ttu-id="a787b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a787b-109">Type</span></span>|<span data-ttu-id="a787b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a787b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a787b-111">девицемоделс</span><span class="sxs-lookup"><span data-stu-id="a787b-111">deviceModels</span></span>|<span data-ttu-id="a787b-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a787b-112">String collection</span></span>|<span data-ttu-id="a787b-113">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="a787b-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="a787b-114">девицемануфактурерс</span><span class="sxs-lookup"><span data-stu-id="a787b-114">deviceManufacturers</span></span>|<span data-ttu-id="a787b-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a787b-115">String collection</span></span>|<span data-ttu-id="a787b-116">Список производства для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="a787b-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="a787b-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="a787b-117">Relationships</span></span>
<span data-ttu-id="a787b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a787b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a787b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a787b-119">JSON Representation</span></span>
<span data-ttu-id="a787b-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a787b-120">Here is a JSON representation of the resource.</span></span>
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



