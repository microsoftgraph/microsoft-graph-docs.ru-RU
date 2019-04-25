---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6867dd6b2243541b193b8b741924487f16ff61c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565977"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="724fb-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="724fb-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="724fb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="724fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="724fb-105">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="724fb-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="724fb-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="724fb-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="724fb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="724fb-107">Properties</span></span>
|<span data-ttu-id="724fb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="724fb-108">Property</span></span>|<span data-ttu-id="724fb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="724fb-109">Type</span></span>|<span data-ttu-id="724fb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="724fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="724fb-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="724fb-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="724fb-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="724fb-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="724fb-113">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="724fb-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="724fb-114">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="724fb-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="724fb-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="724fb-115">Relationships</span></span>
<span data-ttu-id="724fb-116">Нет</span><span class="sxs-lookup"><span data-stu-id="724fb-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="724fb-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="724fb-117">JSON Representation</span></span>
<span data-ttu-id="724fb-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="724fb-118">Here is a JSON representation of the resource.</span></span>
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



