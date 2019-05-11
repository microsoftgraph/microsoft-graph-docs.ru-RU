---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7218e25fc9d1ed0b53bf95cd25ca4b8e3a2e7d8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941942"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="17d08-103">Тип ресурса Манажеддевицемоделсандмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="17d08-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="17d08-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17d08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17d08-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17d08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17d08-106">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="17d08-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="17d08-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="17d08-107">Properties</span></span>
|<span data-ttu-id="17d08-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="17d08-108">Property</span></span>|<span data-ttu-id="17d08-109">Тип</span><span class="sxs-lookup"><span data-stu-id="17d08-109">Type</span></span>|<span data-ttu-id="17d08-110">Описание</span><span class="sxs-lookup"><span data-stu-id="17d08-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17d08-111">Девицемоделс</span><span class="sxs-lookup"><span data-stu-id="17d08-111">deviceModels</span></span>|<span data-ttu-id="17d08-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="17d08-112">String collection</span></span>|<span data-ttu-id="17d08-113">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="17d08-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="17d08-114">Девицемануфактурерс</span><span class="sxs-lookup"><span data-stu-id="17d08-114">deviceManufacturers</span></span>|<span data-ttu-id="17d08-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="17d08-115">String collection</span></span>|<span data-ttu-id="17d08-116">Список производства для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="17d08-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="17d08-117">Связи</span><span class="sxs-lookup"><span data-stu-id="17d08-117">Relationships</span></span>
<span data-ttu-id="17d08-118">Нет</span><span class="sxs-lookup"><span data-stu-id="17d08-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17d08-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17d08-119">JSON Representation</span></span>
<span data-ttu-id="17d08-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17d08-120">Here is a JSON representation of the resource.</span></span>
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




