---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5a2d2152d107050f655d43dab2cb2c65f114868
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031348"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="13ba4-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="13ba4-103">omaSetting resource type</span></span>

> <span data-ttu-id="13ba4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13ba4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13ba4-105">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="13ba4-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="13ba4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="13ba4-106">Properties</span></span>
|<span data-ttu-id="13ba4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="13ba4-107">Property</span></span>|<span data-ttu-id="13ba4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="13ba4-108">Type</span></span>|<span data-ttu-id="13ba4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="13ba4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ba4-110">displayName</span><span class="sxs-lookup"><span data-stu-id="13ba4-110">displayName</span></span>|<span data-ttu-id="13ba4-111">Строка</span><span class="sxs-lookup"><span data-stu-id="13ba4-111">String</span></span>|<span data-ttu-id="13ba4-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="13ba4-112">Display Name.</span></span>|
|<span data-ttu-id="13ba4-113">description</span><span class="sxs-lookup"><span data-stu-id="13ba4-113">description</span></span>|<span data-ttu-id="13ba4-114">String</span><span class="sxs-lookup"><span data-stu-id="13ba4-114">String</span></span>|<span data-ttu-id="13ba4-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="13ba4-115">Description.</span></span>|
|<span data-ttu-id="13ba4-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="13ba4-116">omaUri</span></span>|<span data-ttu-id="13ba4-117">String</span><span class="sxs-lookup"><span data-stu-id="13ba4-117">String</span></span>|<span data-ttu-id="13ba4-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="13ba4-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13ba4-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="13ba4-119">Relationships</span></span>
<span data-ttu-id="13ba4-120">Нет</span><span class="sxs-lookup"><span data-stu-id="13ba4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13ba4-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13ba4-121">JSON Representation</span></span>
<span data-ttu-id="13ba4-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13ba4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



