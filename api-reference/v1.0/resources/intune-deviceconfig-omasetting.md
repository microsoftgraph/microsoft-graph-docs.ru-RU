---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c1b464d8947bfa0125ba7edc9991b7bc6f34296
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367387"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="c5860-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="c5860-103">omaSetting resource type</span></span>

> <span data-ttu-id="c5860-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5860-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5860-105">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="c5860-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c5860-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5860-106">Properties</span></span>
|<span data-ttu-id="c5860-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5860-107">Property</span></span>|<span data-ttu-id="c5860-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c5860-108">Type</span></span>|<span data-ttu-id="c5860-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c5860-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5860-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c5860-110">displayName</span></span>|<span data-ttu-id="c5860-111">Строка</span><span class="sxs-lookup"><span data-stu-id="c5860-111">String</span></span>|<span data-ttu-id="c5860-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c5860-112">Display Name.</span></span>|
|<span data-ttu-id="c5860-113">description</span><span class="sxs-lookup"><span data-stu-id="c5860-113">description</span></span>|<span data-ttu-id="c5860-114">String</span><span class="sxs-lookup"><span data-stu-id="c5860-114">String</span></span>|<span data-ttu-id="c5860-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="c5860-115">Description.</span></span>|
|<span data-ttu-id="c5860-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="c5860-116">omaUri</span></span>|<span data-ttu-id="c5860-117">String</span><span class="sxs-lookup"><span data-stu-id="c5860-117">String</span></span>|<span data-ttu-id="c5860-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="c5860-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5860-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c5860-119">Relationships</span></span>
<span data-ttu-id="c5860-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c5860-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5860-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5860-121">JSON Representation</span></span>
<span data-ttu-id="c5860-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5860-122">Here is a JSON representation of the resource.</span></span>
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




