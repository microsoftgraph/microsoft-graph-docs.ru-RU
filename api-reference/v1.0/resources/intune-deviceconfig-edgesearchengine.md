---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f39793a781a0660da4295bd0c4d69b5b8b305987
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465668"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="64398-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="64398-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="64398-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64398-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64398-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64398-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64398-106">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="64398-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="64398-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="64398-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64398-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="64398-108">Properties</span></span>
|<span data-ttu-id="64398-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="64398-109">Property</span></span>|<span data-ttu-id="64398-110">Тип</span><span class="sxs-lookup"><span data-stu-id="64398-110">Type</span></span>|<span data-ttu-id="64398-111">Описание</span><span class="sxs-lookup"><span data-stu-id="64398-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64398-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="64398-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="64398-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="64398-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="64398-114">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="64398-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="64398-115">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="64398-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64398-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="64398-116">Relationships</span></span>
<span data-ttu-id="64398-117">Нет</span><span class="sxs-lookup"><span data-stu-id="64398-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64398-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64398-118">JSON Representation</span></span>
<span data-ttu-id="64398-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64398-119">Here is a JSON representation of the resource.</span></span>
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







