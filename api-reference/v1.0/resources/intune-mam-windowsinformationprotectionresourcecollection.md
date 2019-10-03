---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 81b3a75533f70c57e31fe0f56770a281b66c61af
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366932"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="b8b19-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="b8b19-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="b8b19-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8b19-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8b19-105">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="b8b19-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="b8b19-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8b19-106">Properties</span></span>
|<span data-ttu-id="b8b19-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8b19-107">Property</span></span>|<span data-ttu-id="b8b19-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b8b19-108">Type</span></span>|<span data-ttu-id="b8b19-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b8b19-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b19-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b8b19-110">displayName</span></span>|<span data-ttu-id="b8b19-111">String</span><span class="sxs-lookup"><span data-stu-id="b8b19-111">String</span></span>|<span data-ttu-id="b8b19-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="b8b19-112">Display name</span></span>|
|<span data-ttu-id="b8b19-113">resources</span><span class="sxs-lookup"><span data-stu-id="b8b19-113">resources</span></span>|<span data-ttu-id="b8b19-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b8b19-114">String collection</span></span>|<span data-ttu-id="b8b19-115">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="b8b19-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8b19-116">Связи</span><span class="sxs-lookup"><span data-stu-id="b8b19-116">Relationships</span></span>
<span data-ttu-id="b8b19-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b8b19-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8b19-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8b19-118">JSON Representation</span></span>
<span data-ttu-id="b8b19-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8b19-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




