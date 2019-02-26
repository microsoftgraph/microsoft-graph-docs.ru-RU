---
title: Тип ресурса resourceAction
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d229a6d4d8b514cbf092efb224ff09dfb0c78ad4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157626"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="d5226-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="d5226-103">resourceAction resource type</span></span>

> <span data-ttu-id="d5226-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5226-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5226-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5226-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5226-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d5226-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d5226-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5226-107">Properties</span></span>
|<span data-ttu-id="d5226-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5226-108">Property</span></span>|<span data-ttu-id="d5226-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d5226-109">Type</span></span>|<span data-ttu-id="d5226-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d5226-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5226-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d5226-111">allowedResourceActions</span></span>|<span data-ttu-id="d5226-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d5226-112">String collection</span></span>|<span data-ttu-id="d5226-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="d5226-113">Allowed Actions</span></span>|
|<span data-ttu-id="d5226-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d5226-114">notAllowedResourceActions</span></span>|<span data-ttu-id="d5226-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d5226-115">String collection</span></span>|<span data-ttu-id="d5226-116">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="d5226-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5226-117">Связи</span><span class="sxs-lookup"><span data-stu-id="d5226-117">Relationships</span></span>
<span data-ttu-id="d5226-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d5226-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5226-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5226-119">JSON Representation</span></span>
<span data-ttu-id="d5226-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5226-120">Here is a JSON representation of the resource.</span></span>
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




