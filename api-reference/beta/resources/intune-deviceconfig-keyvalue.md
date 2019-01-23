---
title: Тип ресурса keyValue
description: Определение значения ключа.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e3133962d9f6bfb5f5363dd6d6cbd4b5ef2ea202
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406817"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="2b340-103">Тип ресурса keyValue</span><span class="sxs-lookup"><span data-stu-id="2b340-103">keyValue resource type</span></span>

> <span data-ttu-id="2b340-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b340-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b340-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b340-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b340-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b340-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b340-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="2b340-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2b340-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b340-108">Properties</span></span>
|<span data-ttu-id="2b340-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b340-109">Property</span></span>|<span data-ttu-id="2b340-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2b340-110">Type</span></span>|<span data-ttu-id="2b340-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2b340-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b340-112">key</span><span class="sxs-lookup"><span data-stu-id="2b340-112">key</span></span>|<span data-ttu-id="2b340-113">String</span><span class="sxs-lookup"><span data-stu-id="2b340-113">String</span></span>|<span data-ttu-id="2b340-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="2b340-114">Key.</span></span>|
|<span data-ttu-id="2b340-115">value</span><span class="sxs-lookup"><span data-stu-id="2b340-115">value</span></span>|<span data-ttu-id="2b340-116">String</span><span class="sxs-lookup"><span data-stu-id="2b340-116">String</span></span>|<span data-ttu-id="2b340-117">Значение</span><span class="sxs-lookup"><span data-stu-id="2b340-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b340-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2b340-118">Relationships</span></span>
<span data-ttu-id="2b340-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2b340-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b340-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b340-120">JSON Representation</span></span>
<span data-ttu-id="2b340-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b340-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```




