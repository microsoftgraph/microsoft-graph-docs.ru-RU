---
title: Тип ресурса Ключзначение
description: Определение значения ключа.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86a18d434722cff9b6737dd14a83e8aa38ed102c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439878"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="7554b-103">Тип ресурса Ключзначение</span><span class="sxs-lookup"><span data-stu-id="7554b-103">keyValue resource type</span></span>

<span data-ttu-id="7554b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7554b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7554b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7554b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7554b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7554b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7554b-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="7554b-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="7554b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7554b-108">Properties</span></span>
|<span data-ttu-id="7554b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7554b-109">Property</span></span>|<span data-ttu-id="7554b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7554b-110">Type</span></span>|<span data-ttu-id="7554b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7554b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7554b-112">ключа</span><span class="sxs-lookup"><span data-stu-id="7554b-112">key</span></span>|<span data-ttu-id="7554b-113">String</span><span class="sxs-lookup"><span data-stu-id="7554b-113">String</span></span>|<span data-ttu-id="7554b-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="7554b-114">Key.</span></span>|
|<span data-ttu-id="7554b-115">value</span><span class="sxs-lookup"><span data-stu-id="7554b-115">value</span></span>|<span data-ttu-id="7554b-116">String</span><span class="sxs-lookup"><span data-stu-id="7554b-116">String</span></span>|<span data-ttu-id="7554b-117">Значение</span><span class="sxs-lookup"><span data-stu-id="7554b-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7554b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="7554b-118">Relationships</span></span>
<span data-ttu-id="7554b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7554b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7554b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7554b-120">JSON Representation</span></span>
<span data-ttu-id="7554b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7554b-121">Here is a JSON representation of the resource.</span></span>
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



