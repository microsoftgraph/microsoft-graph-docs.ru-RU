---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ac83d2501eb42cc12044e8d566031e6a5dd6080c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783958"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="f7251-103">Тип ресурса Манажеддевицемоделсандмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="f7251-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="f7251-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7251-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7251-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7251-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7251-106">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="f7251-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="f7251-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7251-107">Properties</span></span>
|<span data-ttu-id="f7251-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7251-108">Property</span></span>|<span data-ttu-id="f7251-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f7251-109">Type</span></span>|<span data-ttu-id="f7251-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f7251-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7251-111">девицемоделс</span><span class="sxs-lookup"><span data-stu-id="f7251-111">deviceModels</span></span>|<span data-ttu-id="f7251-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f7251-112">String collection</span></span>|<span data-ttu-id="f7251-113">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="f7251-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="f7251-114">девицемануфактурерс</span><span class="sxs-lookup"><span data-stu-id="f7251-114">deviceManufacturers</span></span>|<span data-ttu-id="f7251-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f7251-115">String collection</span></span>|<span data-ttu-id="f7251-116">Список производства для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="f7251-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7251-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f7251-117">Relationships</span></span>
<span data-ttu-id="f7251-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f7251-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7251-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7251-119">JSON Representation</span></span>
<span data-ttu-id="f7251-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7251-120">Here is a JSON representation of the resource.</span></span>
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



