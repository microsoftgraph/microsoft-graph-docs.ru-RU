---
title: Тип ресурса Манажеддевицемоделсандмануфактурерс
description: Модели и производства меатадата для управляемых устройств в учетной записи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: afcd9ea210d50bd5778133fcac743ba7bd624118
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725472"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="f13e2-103">Тип ресурса Манажеддевицемоделсандмануфактурерс</span><span class="sxs-lookup"><span data-stu-id="f13e2-103">managedDeviceModelsAndManufacturers resource type</span></span>

<span data-ttu-id="f13e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f13e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f13e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f13e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f13e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f13e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f13e2-107">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="f13e2-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="f13e2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f13e2-108">Properties</span></span>
|<span data-ttu-id="f13e2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f13e2-109">Property</span></span>|<span data-ttu-id="f13e2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f13e2-110">Type</span></span>|<span data-ttu-id="f13e2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f13e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f13e2-112">девицемоделс</span><span class="sxs-lookup"><span data-stu-id="f13e2-112">deviceModels</span></span>|<span data-ttu-id="f13e2-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f13e2-113">String collection</span></span>|<span data-ttu-id="f13e2-114">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="f13e2-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="f13e2-115">девицемануфактурерс</span><span class="sxs-lookup"><span data-stu-id="f13e2-115">deviceManufacturers</span></span>|<span data-ttu-id="f13e2-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f13e2-116">String collection</span></span>|<span data-ttu-id="f13e2-117">Список производства для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="f13e2-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="f13e2-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f13e2-118">Relationships</span></span>
<span data-ttu-id="f13e2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f13e2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f13e2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f13e2-120">JSON Representation</span></span>
<span data-ttu-id="f13e2-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f13e2-121">Here is a JSON representation of the resource.</span></span>
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





