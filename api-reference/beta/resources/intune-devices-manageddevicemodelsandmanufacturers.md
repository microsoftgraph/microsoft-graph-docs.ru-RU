---
title: Тип ресурса managedDeviceModelsAndManufacturers
description: Модели и производители meatadata для управляемых устройств в учетной записи
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afcf64cb0e8db4e24ce061490ecc593595690930
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396793"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="8ba4b-103">Тип ресурса managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="8ba4b-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="8ba4b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ba4b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8ba4b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ba4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ba4b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ba4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ba4b-107">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="8ba4b-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="8ba4b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ba4b-108">Properties</span></span>
|<span data-ttu-id="8ba4b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ba4b-109">Property</span></span>|<span data-ttu-id="8ba4b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8ba4b-110">Type</span></span>|<span data-ttu-id="8ba4b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ba4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ba4b-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="8ba4b-112">deviceModels</span></span>|<span data-ttu-id="8ba4b-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8ba4b-113">String collection</span></span>|<span data-ttu-id="8ba4b-114">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="8ba4b-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="8ba4b-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="8ba4b-115">deviceManufacturers</span></span>|<span data-ttu-id="8ba4b-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8ba4b-116">String collection</span></span>|<span data-ttu-id="8ba4b-117">Список производители управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="8ba4b-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ba4b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="8ba4b-118">Relationships</span></span>
<span data-ttu-id="8ba4b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8ba4b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ba4b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ba4b-120">JSON Representation</span></span>
<span data-ttu-id="8ba4b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ba4b-121">Here is a JSON representation of the resource.</span></span>
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




