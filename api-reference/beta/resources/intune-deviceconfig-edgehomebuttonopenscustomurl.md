---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c3fa2465200b216e3519b4eb15700406bd67f16
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332549"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="af3fd-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="af3fd-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="af3fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af3fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af3fd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af3fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af3fd-106">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="af3fd-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="af3fd-107">Наследуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af3fd-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af3fd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="af3fd-108">Properties</span></span>
|<span data-ttu-id="af3fd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="af3fd-109">Property</span></span>|<span data-ttu-id="af3fd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="af3fd-110">Type</span></span>|<span data-ttu-id="af3fd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="af3fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af3fd-112">хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="af3fd-112">homeButtonCustomURL</span></span>|<span data-ttu-id="af3fd-113">String</span><span class="sxs-lookup"><span data-stu-id="af3fd-113">String</span></span>|<span data-ttu-id="af3fd-114">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="af3fd-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af3fd-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="af3fd-115">Relationships</span></span>
<span data-ttu-id="af3fd-116">Нет</span><span class="sxs-lookup"><span data-stu-id="af3fd-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af3fd-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af3fd-117">JSON Representation</span></span>
<span data-ttu-id="af3fd-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af3fd-118">Here is a JSON representation of the resource.</span></span>
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



