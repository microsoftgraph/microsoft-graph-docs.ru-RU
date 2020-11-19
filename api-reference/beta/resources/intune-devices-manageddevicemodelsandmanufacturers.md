---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6ed8f1d2bc55e05edc54c3ec19d84c5d7fc46e96
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208823"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="9d3bb-103">Тип ресурса Манажеддевицемоделсандмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="9d3bb-103">managedDeviceModelsAndManufacturers resource type</span></span>

<span data-ttu-id="9d3bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d3bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d3bb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d3bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d3bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d3bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d3bb-107">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="9d3bb-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="9d3bb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d3bb-108">Properties</span></span>
|<span data-ttu-id="9d3bb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d3bb-109">Property</span></span>|<span data-ttu-id="9d3bb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9d3bb-110">Type</span></span>|<span data-ttu-id="9d3bb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9d3bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d3bb-112">девицемоделс</span><span class="sxs-lookup"><span data-stu-id="9d3bb-112">deviceModels</span></span>|<span data-ttu-id="9d3bb-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9d3bb-113">String collection</span></span>|<span data-ttu-id="9d3bb-114">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="9d3bb-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="9d3bb-115">девицемануфактурерс</span><span class="sxs-lookup"><span data-stu-id="9d3bb-115">deviceManufacturers</span></span>|<span data-ttu-id="9d3bb-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9d3bb-116">String collection</span></span>|<span data-ttu-id="9d3bb-117">Список производства для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="9d3bb-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d3bb-118">Связи</span><span class="sxs-lookup"><span data-stu-id="9d3bb-118">Relationships</span></span>
<span data-ttu-id="9d3bb-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9d3bb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d3bb-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d3bb-120">JSON Representation</span></span>
<span data-ttu-id="9d3bb-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d3bb-121">Here is a JSON representation of the resource.</span></span>
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




