---
title: Тип ресурса managedDeviceModelsAndManufacturers
description: Модели и производители meatadata для управляемых устройств в учетной записи
author: tfitzmac
ms.openlocfilehash: 42611b0c14aa583d2871d97b66ce116a0b835268
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352936"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="abbbd-103">Тип ресурса managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="abbbd-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="abbbd-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="abbbd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abbbd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abbbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abbbd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="abbbd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abbbd-107">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="abbbd-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="abbbd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="abbbd-108">Properties</span></span>
|<span data-ttu-id="abbbd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="abbbd-109">Property</span></span>|<span data-ttu-id="abbbd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="abbbd-110">Type</span></span>|<span data-ttu-id="abbbd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="abbbd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abbbd-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="abbbd-112">deviceModels</span></span>|<span data-ttu-id="abbbd-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="abbbd-113">String collection</span></span>|<span data-ttu-id="abbbd-114">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="abbbd-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="abbbd-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="abbbd-115">deviceManufacturers</span></span>|<span data-ttu-id="abbbd-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="abbbd-116">String collection</span></span>|<span data-ttu-id="abbbd-117">Список производители управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="abbbd-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="abbbd-118">Связи</span><span class="sxs-lookup"><span data-stu-id="abbbd-118">Relationships</span></span>
<span data-ttu-id="abbbd-119">Нет</span><span class="sxs-lookup"><span data-stu-id="abbbd-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="abbbd-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="abbbd-120">JSON Representation</span></span>
<span data-ttu-id="abbbd-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abbbd-121">Here is a JSON representation of the resource.</span></span>
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





