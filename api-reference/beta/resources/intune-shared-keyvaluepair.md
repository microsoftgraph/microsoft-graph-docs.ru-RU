---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f31e83c5e53ea4c2873fd2b425cc0e0c02678ea7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415784"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="ed1a3-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="ed1a3-103">keyValuePair resource type</span></span>

> <span data-ttu-id="ed1a3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed1a3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ed1a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed1a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed1a3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed1a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed1a3-107">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="ed1a3-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="ed1a3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed1a3-108">Properties</span></span>
|<span data-ttu-id="ed1a3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed1a3-109">Property</span></span>|<span data-ttu-id="ed1a3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ed1a3-110">Type</span></span>|<span data-ttu-id="ed1a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed1a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed1a3-112">name</span><span class="sxs-lookup"><span data-stu-id="ed1a3-112">name</span></span>|<span data-ttu-id="ed1a3-113">String</span><span class="sxs-lookup"><span data-stu-id="ed1a3-113">String</span></span>|<span data-ttu-id="ed1a3-114">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="ed1a3-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="ed1a3-115">value</span><span class="sxs-lookup"><span data-stu-id="ed1a3-115">value</span></span>|<span data-ttu-id="ed1a3-116">String</span><span class="sxs-lookup"><span data-stu-id="ed1a3-116">String</span></span>|<span data-ttu-id="ed1a3-117">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="ed1a3-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed1a3-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ed1a3-118">Relationships</span></span>
<span data-ttu-id="ed1a3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ed1a3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed1a3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed1a3-120">JSON Representation</span></span>
<span data-ttu-id="ed1a3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed1a3-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```




