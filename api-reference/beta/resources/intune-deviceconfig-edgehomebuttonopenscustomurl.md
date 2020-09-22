---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4779de3f0a6e53b8056a42e1df511ea176dd6378
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058237"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="ebce2-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="ebce2-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="ebce2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebce2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebce2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebce2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebce2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebce2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebce2-107">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="ebce2-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="ebce2-108">Наследуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebce2-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ebce2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebce2-109">Properties</span></span>
|<span data-ttu-id="ebce2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebce2-110">Property</span></span>|<span data-ttu-id="ebce2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ebce2-111">Type</span></span>|<span data-ttu-id="ebce2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ebce2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebce2-113">хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="ebce2-113">homeButtonCustomURL</span></span>|<span data-ttu-id="ebce2-114">String</span><span class="sxs-lookup"><span data-stu-id="ebce2-114">String</span></span>|<span data-ttu-id="ebce2-115">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="ebce2-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebce2-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ebce2-116">Relationships</span></span>
<span data-ttu-id="ebce2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ebce2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebce2-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebce2-118">JSON Representation</span></span>
<span data-ttu-id="ebce2-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebce2-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```






