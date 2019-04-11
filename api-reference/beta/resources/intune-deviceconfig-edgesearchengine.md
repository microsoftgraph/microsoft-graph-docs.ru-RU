---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86604849a488f9f9bf8626f8bfba205efd11a532
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782767"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="190f7-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="190f7-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="190f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="190f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="190f7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="190f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="190f7-106">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="190f7-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="190f7-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="190f7-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="190f7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="190f7-108">Properties</span></span>
|<span data-ttu-id="190f7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="190f7-109">Property</span></span>|<span data-ttu-id="190f7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="190f7-110">Type</span></span>|<span data-ttu-id="190f7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="190f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="190f7-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="190f7-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="190f7-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="190f7-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="190f7-114">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="190f7-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="190f7-115">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="190f7-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="190f7-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="190f7-116">Relationships</span></span>
<span data-ttu-id="190f7-117">Нет</span><span class="sxs-lookup"><span data-stu-id="190f7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="190f7-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="190f7-118">JSON Representation</span></span>
<span data-ttu-id="190f7-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="190f7-119">Here is a JSON representation of the resource.</span></span>
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





