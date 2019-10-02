---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a3e03bd601bbe6ad037ee59227ca2ed9ab5cb611
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359343"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="917e9-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="917e9-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="917e9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="917e9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="917e9-105">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="917e9-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="917e9-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="917e9-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="917e9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="917e9-107">Properties</span></span>
|<span data-ttu-id="917e9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="917e9-108">Property</span></span>|<span data-ttu-id="917e9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="917e9-109">Type</span></span>|<span data-ttu-id="917e9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="917e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="917e9-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="917e9-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="917e9-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="917e9-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="917e9-113">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="917e9-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="917e9-114">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="917e9-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="917e9-115">Связи</span><span class="sxs-lookup"><span data-stu-id="917e9-115">Relationships</span></span>
<span data-ttu-id="917e9-116">Нет</span><span class="sxs-lookup"><span data-stu-id="917e9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="917e9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="917e9-117">JSON Representation</span></span>
<span data-ttu-id="917e9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="917e9-118">Here is a JSON representation of the resource.</span></span>
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




