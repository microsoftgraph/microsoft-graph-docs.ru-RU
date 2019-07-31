---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 750208cd58a70912a437fc17ee4e2b7cc218543e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001413"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="0d901-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="0d901-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="0d901-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d901-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d901-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d901-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d901-106">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="0d901-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="0d901-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="0d901-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d901-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d901-108">Properties</span></span>
|<span data-ttu-id="0d901-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d901-109">Property</span></span>|<span data-ttu-id="0d901-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0d901-110">Type</span></span>|<span data-ttu-id="0d901-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d901-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d901-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="0d901-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="0d901-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="0d901-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="0d901-114">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="0d901-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="0d901-115">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="0d901-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d901-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="0d901-116">Relationships</span></span>
<span data-ttu-id="0d901-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0d901-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d901-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d901-118">JSON Representation</span></span>
<span data-ttu-id="0d901-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d901-119">Here is a JSON representation of the resource.</span></span>
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





