---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5ea2d73724400c033a3bd8e1148e04af8d390be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755072"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="e3b6d-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="e3b6d-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="e3b6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3b6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3b6d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3b6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3b6d-106">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="e3b6d-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="e3b6d-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="e3b6d-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3b6d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3b6d-108">Properties</span></span>
|<span data-ttu-id="e3b6d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3b6d-109">Property</span></span>|<span data-ttu-id="e3b6d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e3b6d-110">Type</span></span>|<span data-ttu-id="e3b6d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e3b6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3b6d-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="e3b6d-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="e3b6d-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="e3b6d-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="e3b6d-114">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="e3b6d-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="e3b6d-115">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="e3b6d-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3b6d-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="e3b6d-116">Relationships</span></span>
<span data-ttu-id="e3b6d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="e3b6d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3b6d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3b6d-118">JSON Representation</span></span>
<span data-ttu-id="e3b6d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3b6d-119">Here is a JSON representation of the resource.</span></span>
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




