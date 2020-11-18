---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 619c925ff58745054a4cc62c638f1776ee96d5f2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199016"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="f2b0c-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="f2b0c-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="f2b0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2b0c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2b0c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2b0c-107">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="f2b0c-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="f2b0c-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2b0c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2b0c-109">Properties</span></span>
|<span data-ttu-id="f2b0c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2b0c-110">Property</span></span>|<span data-ttu-id="f2b0c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f2b0c-111">Type</span></span>|<span data-ttu-id="f2b0c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f2b0c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2b0c-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="f2b0c-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="f2b0c-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="f2b0c-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="f2b0c-115">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="f2b0c-116">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2b0c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f2b0c-117">Relationships</span></span>
<span data-ttu-id="f2b0c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f2b0c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2b0c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2b0c-119">JSON Representation</span></span>
<span data-ttu-id="f2b0c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2b0c-120">Here is a JSON representation of the resource.</span></span>
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




