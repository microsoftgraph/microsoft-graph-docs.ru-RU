---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9471c92dc88d49426a7f8c41f73708594b7cbf8c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791865"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="4850a-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="4850a-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="4850a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4850a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4850a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4850a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4850a-106">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="4850a-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="4850a-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="4850a-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4850a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4850a-108">Properties</span></span>
|<span data-ttu-id="4850a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4850a-109">Property</span></span>|<span data-ttu-id="4850a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4850a-110">Type</span></span>|<span data-ttu-id="4850a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4850a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4850a-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="4850a-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="4850a-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="4850a-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="4850a-114">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="4850a-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="4850a-115">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="4850a-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4850a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4850a-116">Relationships</span></span>
<span data-ttu-id="4850a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4850a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4850a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4850a-118">JSON Representation</span></span>
<span data-ttu-id="4850a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4850a-119">Here is a JSON representation of the resource.</span></span>
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



