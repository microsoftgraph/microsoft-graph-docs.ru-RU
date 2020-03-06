---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1be131396c67f5af37a10ab3e0b7b1248cc8c4bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532547"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="a65d7-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="a65d7-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="a65d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a65d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a65d7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a65d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a65d7-106">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="a65d7-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="a65d7-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="a65d7-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a65d7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a65d7-108">Properties</span></span>
|<span data-ttu-id="a65d7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a65d7-109">Property</span></span>|<span data-ttu-id="a65d7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a65d7-110">Type</span></span>|<span data-ttu-id="a65d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a65d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a65d7-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a65d7-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="a65d7-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a65d7-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="a65d7-114">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="a65d7-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="a65d7-115">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="a65d7-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a65d7-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a65d7-116">Relationships</span></span>
<span data-ttu-id="a65d7-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a65d7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a65d7-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a65d7-118">JSON Representation</span></span>
<span data-ttu-id="a65d7-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a65d7-119">Here is a JSON representation of the resource.</span></span>
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




