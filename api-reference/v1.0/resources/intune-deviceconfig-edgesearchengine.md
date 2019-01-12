---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 87a072ca6fb325f599c51a219bfa0e9d2ad0ac0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935621"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="15ebb-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="15ebb-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="15ebb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="15ebb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15ebb-105">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="15ebb-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="15ebb-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="15ebb-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15ebb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="15ebb-107">Properties</span></span>
|<span data-ttu-id="15ebb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="15ebb-108">Property</span></span>|<span data-ttu-id="15ebb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="15ebb-109">Type</span></span>|<span data-ttu-id="15ebb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15ebb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ebb-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="15ebb-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="15ebb-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="15ebb-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="15ebb-113">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="15ebb-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="15ebb-114">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="15ebb-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15ebb-115">Связи</span><span class="sxs-lookup"><span data-stu-id="15ebb-115">Relationships</span></span>
<span data-ttu-id="15ebb-116">Нет</span><span class="sxs-lookup"><span data-stu-id="15ebb-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15ebb-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15ebb-117">JSON Representation</span></span>
<span data-ttu-id="15ebb-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15ebb-118">Here is a JSON representation of the resource.</span></span>
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



