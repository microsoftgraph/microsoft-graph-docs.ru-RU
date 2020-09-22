---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 040ff093004cdb1d31dde748a7ad26f03ce08b10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056795"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="66a25-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="66a25-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="66a25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66a25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66a25-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66a25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66a25-106">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="66a25-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="66a25-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="66a25-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66a25-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="66a25-108">Properties</span></span>
|<span data-ttu-id="66a25-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="66a25-109">Property</span></span>|<span data-ttu-id="66a25-110">Тип</span><span class="sxs-lookup"><span data-stu-id="66a25-110">Type</span></span>|<span data-ttu-id="66a25-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66a25-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66a25-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="66a25-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="66a25-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="66a25-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="66a25-114">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="66a25-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="66a25-115">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="66a25-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66a25-116">Связи</span><span class="sxs-lookup"><span data-stu-id="66a25-116">Relationships</span></span>
<span data-ttu-id="66a25-117">Нет</span><span class="sxs-lookup"><span data-stu-id="66a25-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66a25-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66a25-118">JSON Representation</span></span>
<span data-ttu-id="66a25-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66a25-119">Here is a JSON representation of the resource.</span></span>
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









