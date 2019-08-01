---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d733abca0dd390e83e51b25afd1ba7e86886b3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028380"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="3f0cb-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="3f0cb-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="3f0cb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f0cb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f0cb-105">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="3f0cb-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="3f0cb-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="3f0cb-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f0cb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f0cb-107">Properties</span></span>
|<span data-ttu-id="3f0cb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f0cb-108">Property</span></span>|<span data-ttu-id="3f0cb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3f0cb-109">Type</span></span>|<span data-ttu-id="3f0cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3f0cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f0cb-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="3f0cb-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="3f0cb-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="3f0cb-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="3f0cb-113">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="3f0cb-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="3f0cb-114">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="3f0cb-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f0cb-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="3f0cb-115">Relationships</span></span>
<span data-ttu-id="3f0cb-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3f0cb-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f0cb-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f0cb-117">JSON Representation</span></span>
<span data-ttu-id="3f0cb-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f0cb-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



