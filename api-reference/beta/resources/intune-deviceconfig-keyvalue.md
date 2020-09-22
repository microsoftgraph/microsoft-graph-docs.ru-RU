---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b6d42009d03bfa88007688065d68099598f1e6eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003607"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="23bc5-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="23bc5-103">keyValue resource type</span></span>

<span data-ttu-id="23bc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23bc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23bc5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23bc5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23bc5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23bc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23bc5-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="23bc5-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="23bc5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="23bc5-108">Properties</span></span>
|<span data-ttu-id="23bc5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="23bc5-109">Property</span></span>|<span data-ttu-id="23bc5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="23bc5-110">Type</span></span>|<span data-ttu-id="23bc5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23bc5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23bc5-112">key</span><span class="sxs-lookup"><span data-stu-id="23bc5-112">key</span></span>|<span data-ttu-id="23bc5-113">String</span><span class="sxs-lookup"><span data-stu-id="23bc5-113">String</span></span>|<span data-ttu-id="23bc5-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="23bc5-114">Key.</span></span>|
|<span data-ttu-id="23bc5-115">value</span><span class="sxs-lookup"><span data-stu-id="23bc5-115">value</span></span>|<span data-ttu-id="23bc5-116">String</span><span class="sxs-lookup"><span data-stu-id="23bc5-116">String</span></span>|<span data-ttu-id="23bc5-117">Значение</span><span class="sxs-lookup"><span data-stu-id="23bc5-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23bc5-118">Связи</span><span class="sxs-lookup"><span data-stu-id="23bc5-118">Relationships</span></span>
<span data-ttu-id="23bc5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="23bc5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23bc5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23bc5-120">JSON Representation</span></span>
<span data-ttu-id="23bc5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23bc5-121">Here is a JSON representation of the resource.</span></span>
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






