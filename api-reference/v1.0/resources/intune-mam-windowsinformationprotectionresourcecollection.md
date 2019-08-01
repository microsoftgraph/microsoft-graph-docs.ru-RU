---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 754f5ce902ca4cb5bb63be41f0e8094cc0738c26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037641"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="7f23d-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="7f23d-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="7f23d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f23d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f23d-105">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="7f23d-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="7f23d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f23d-106">Properties</span></span>
|<span data-ttu-id="7f23d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f23d-107">Property</span></span>|<span data-ttu-id="7f23d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7f23d-108">Type</span></span>|<span data-ttu-id="7f23d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7f23d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f23d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7f23d-110">displayName</span></span>|<span data-ttu-id="7f23d-111">String</span><span class="sxs-lookup"><span data-stu-id="7f23d-111">String</span></span>|<span data-ttu-id="7f23d-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="7f23d-112">Display name</span></span>|
|<span data-ttu-id="7f23d-113">resources</span><span class="sxs-lookup"><span data-stu-id="7f23d-113">resources</span></span>|<span data-ttu-id="7f23d-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7f23d-114">String collection</span></span>|<span data-ttu-id="7f23d-115">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="7f23d-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f23d-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="7f23d-116">Relationships</span></span>
<span data-ttu-id="7f23d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="7f23d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f23d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f23d-118">JSON Representation</span></span>
<span data-ttu-id="7f23d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f23d-119">Here is a JSON representation of the resource.</span></span>
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



