---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1b7b689bcffb8950fd75e244089b7d9c74ad9ace
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081218"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="95979-103">Тип ресурса Манажеддевицемоделсандмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="95979-103">managedDeviceModelsAndManufacturers resource type</span></span>

<span data-ttu-id="95979-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95979-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95979-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95979-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95979-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95979-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95979-107">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="95979-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="95979-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="95979-108">Properties</span></span>
|<span data-ttu-id="95979-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="95979-109">Property</span></span>|<span data-ttu-id="95979-110">Тип</span><span class="sxs-lookup"><span data-stu-id="95979-110">Type</span></span>|<span data-ttu-id="95979-111">Описание</span><span class="sxs-lookup"><span data-stu-id="95979-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95979-112">девицемоделс</span><span class="sxs-lookup"><span data-stu-id="95979-112">deviceModels</span></span>|<span data-ttu-id="95979-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95979-113">String collection</span></span>|<span data-ttu-id="95979-114">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="95979-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="95979-115">девицемануфактурерс</span><span class="sxs-lookup"><span data-stu-id="95979-115">deviceManufacturers</span></span>|<span data-ttu-id="95979-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95979-116">String collection</span></span>|<span data-ttu-id="95979-117">Список производства для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="95979-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="95979-118">Связи</span><span class="sxs-lookup"><span data-stu-id="95979-118">Relationships</span></span>
<span data-ttu-id="95979-119">Нет</span><span class="sxs-lookup"><span data-stu-id="95979-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95979-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95979-120">JSON Representation</span></span>
<span data-ttu-id="95979-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95979-121">Here is a JSON representation of the resource.</span></span>
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






