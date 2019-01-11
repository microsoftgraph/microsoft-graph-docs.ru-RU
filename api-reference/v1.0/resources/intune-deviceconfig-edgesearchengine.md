---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7a58cbed251773559beb2589893ab9759d4758fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819910"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="7b7c8-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="7b7c8-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="7b7c8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b7c8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b7c8-105">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="7b7c8-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="7b7c8-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="7b7c8-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7b7c8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b7c8-107">Properties</span></span>
|<span data-ttu-id="7b7c8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b7c8-108">Property</span></span>|<span data-ttu-id="7b7c8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b7c8-109">Type</span></span>|<span data-ttu-id="7b7c8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b7c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b7c8-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7b7c8-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="7b7c8-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7b7c8-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="7b7c8-113">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="7b7c8-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="7b7c8-114">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="7b7c8-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b7c8-115">Связи</span><span class="sxs-lookup"><span data-stu-id="7b7c8-115">Relationships</span></span>
<span data-ttu-id="7b7c8-116">Нет</span><span class="sxs-lookup"><span data-stu-id="7b7c8-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7b7c8-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b7c8-117">JSON Representation</span></span>
<span data-ttu-id="7b7c8-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b7c8-118">Here is a JSON representation of the resource.</span></span>
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



