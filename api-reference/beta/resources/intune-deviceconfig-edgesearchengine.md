---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9828d2540f1b386302c18cde67811fe06fd9e50f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530049"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="1d857-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="1d857-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="1d857-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1d857-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d857-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d857-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d857-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d857-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d857-107">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="1d857-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="1d857-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="1d857-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1d857-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d857-109">Properties</span></span>
|<span data-ttu-id="1d857-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d857-110">Property</span></span>|<span data-ttu-id="1d857-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1d857-111">Type</span></span>|<span data-ttu-id="1d857-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1d857-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d857-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="1d857-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="1d857-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="1d857-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="1d857-115">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="1d857-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="1d857-116">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="1d857-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d857-117">Связи</span><span class="sxs-lookup"><span data-stu-id="1d857-117">Relationships</span></span>
<span data-ttu-id="1d857-118">Нет</span><span class="sxs-lookup"><span data-stu-id="1d857-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d857-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d857-119">JSON Representation</span></span>
<span data-ttu-id="1d857-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d857-120">Here is a JSON representation of the resource.</span></span>
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



