---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
ms.openlocfilehash: 4da5008eda31bb393ed25048c5d94724d2174e3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026123"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="f3de7-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="f3de7-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="f3de7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f3de7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3de7-105">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="f3de7-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="f3de7-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="f3de7-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3de7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3de7-107">Properties</span></span>
|<span data-ttu-id="f3de7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3de7-108">Property</span></span>|<span data-ttu-id="f3de7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3de7-109">Type</span></span>|<span data-ttu-id="f3de7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3de7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3de7-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="f3de7-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="f3de7-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="f3de7-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="f3de7-113">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="f3de7-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="f3de7-114">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="f3de7-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3de7-115">Связи</span><span class="sxs-lookup"><span data-stu-id="f3de7-115">Relationships</span></span>
<span data-ttu-id="f3de7-116">Нет</span><span class="sxs-lookup"><span data-stu-id="f3de7-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3de7-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3de7-117">JSON Representation</span></span>
<span data-ttu-id="f3de7-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3de7-118">Here is a JSON representation of the resource.</span></span>
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



