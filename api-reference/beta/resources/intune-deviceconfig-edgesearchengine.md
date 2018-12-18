---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: tfitzmac
ms.openlocfilehash: bbe5ba35c9d5832a1910414f99a4de4e9fa957e2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361231"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="7caac-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="7caac-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="7caac-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7caac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7caac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7caac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7caac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7caac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7caac-107">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="7caac-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="7caac-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="7caac-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7caac-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7caac-109">Properties</span></span>
|<span data-ttu-id="7caac-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7caac-110">Property</span></span>|<span data-ttu-id="7caac-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7caac-111">Type</span></span>|<span data-ttu-id="7caac-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7caac-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7caac-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7caac-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="7caac-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7caac-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="7caac-115">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="7caac-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="7caac-116">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="7caac-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7caac-117">Связи</span><span class="sxs-lookup"><span data-stu-id="7caac-117">Relationships</span></span>
<span data-ttu-id="7caac-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7caac-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7caac-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7caac-119">JSON Representation</span></span>
<span data-ttu-id="7caac-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7caac-120">Here is a JSON representation of the resource.</span></span>
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





