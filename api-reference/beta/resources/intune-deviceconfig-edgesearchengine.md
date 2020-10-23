---
title: Тип ресурса edgeSearchEngine
description: Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 615c2d70dcde39a729bcbeff3175130b27aed108
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728607"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="89993-103">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="89993-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="89993-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89993-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89993-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89993-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89993-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89993-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89993-107">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="89993-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="89993-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="89993-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="89993-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="89993-109">Properties</span></span>
|<span data-ttu-id="89993-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="89993-110">Property</span></span>|<span data-ttu-id="89993-111">Тип</span><span class="sxs-lookup"><span data-stu-id="89993-111">Type</span></span>|<span data-ttu-id="89993-112">Описание</span><span class="sxs-lookup"><span data-stu-id="89993-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89993-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="89993-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="89993-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="89993-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="89993-115">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="89993-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="89993-116">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="89993-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89993-117">Связи</span><span class="sxs-lookup"><span data-stu-id="89993-117">Relationships</span></span>
<span data-ttu-id="89993-118">Нет</span><span class="sxs-lookup"><span data-stu-id="89993-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89993-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89993-119">JSON Representation</span></span>
<span data-ttu-id="89993-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89993-120">Here is a JSON representation of the resource.</span></span>
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





