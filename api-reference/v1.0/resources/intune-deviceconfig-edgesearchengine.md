---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6867dd6b2243541b193b8b741924487f16ff61c5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254473"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="7bf31-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="7bf31-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="7bf31-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bf31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bf31-105">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="7bf31-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="7bf31-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="7bf31-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7bf31-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bf31-107">Properties</span></span>
|<span data-ttu-id="7bf31-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bf31-108">Property</span></span>|<span data-ttu-id="7bf31-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7bf31-109">Type</span></span>|<span data-ttu-id="7bf31-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7bf31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bf31-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7bf31-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="7bf31-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7bf31-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="7bf31-113">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="7bf31-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="7bf31-114">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="7bf31-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bf31-115">Связи</span><span class="sxs-lookup"><span data-stu-id="7bf31-115">Relationships</span></span>
<span data-ttu-id="7bf31-116">Нет</span><span class="sxs-lookup"><span data-stu-id="7bf31-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bf31-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bf31-117">JSON Representation</span></span>
<span data-ttu-id="7bf31-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bf31-118">Here is a JSON representation of the resource.</span></span>
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



