---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9808e5f1c51c6893159d1c04c1fae967e83cef64
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386176"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="3ed95-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="3ed95-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="3ed95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ed95-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ed95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ed95-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ed95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ed95-107">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="3ed95-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="3ed95-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="3ed95-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ed95-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ed95-109">Properties</span></span>
|<span data-ttu-id="3ed95-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ed95-110">Property</span></span>|<span data-ttu-id="3ed95-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3ed95-111">Type</span></span>|<span data-ttu-id="3ed95-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3ed95-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ed95-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="3ed95-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="3ed95-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="3ed95-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="3ed95-115">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="3ed95-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="3ed95-116">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="3ed95-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ed95-117">Связи</span><span class="sxs-lookup"><span data-stu-id="3ed95-117">Relationships</span></span>
<span data-ttu-id="3ed95-118">Нет</span><span class="sxs-lookup"><span data-stu-id="3ed95-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ed95-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ed95-119">JSON Representation</span></span>
<span data-ttu-id="3ed95-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ed95-120">Here is a JSON representation of the resource.</span></span>
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



