---
title: Тип ресурса resourceAction
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5442ed8ee55005b1261da09d999e9c27053276d2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415266"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="fc3c9-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="fc3c9-103">resourceAction resource type</span></span>

> <span data-ttu-id="fc3c9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc3c9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc3c9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc3c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc3c9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc3c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc3c9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fc3c9-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fc3c9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc3c9-108">Properties</span></span>
|<span data-ttu-id="fc3c9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc3c9-109">Property</span></span>|<span data-ttu-id="fc3c9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fc3c9-110">Type</span></span>|<span data-ttu-id="fc3c9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc3c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc3c9-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="fc3c9-112">allowedResourceActions</span></span>|<span data-ttu-id="fc3c9-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc3c9-113">String collection</span></span>|<span data-ttu-id="fc3c9-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="fc3c9-114">Allowed Actions</span></span>|
|<span data-ttu-id="fc3c9-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="fc3c9-115">notAllowedResourceActions</span></span>|<span data-ttu-id="fc3c9-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc3c9-116">String collection</span></span>|<span data-ttu-id="fc3c9-117">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="fc3c9-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc3c9-118">Связи</span><span class="sxs-lookup"><span data-stu-id="fc3c9-118">Relationships</span></span>
<span data-ttu-id="fc3c9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="fc3c9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc3c9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc3c9-120">JSON Representation</span></span>
<span data-ttu-id="fc3c9-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc3c9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




