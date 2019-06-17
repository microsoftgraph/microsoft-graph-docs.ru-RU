---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f16f883622ace795628d7c34214cc4b5d12017e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989797"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="dce2d-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="dce2d-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="dce2d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dce2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dce2d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dce2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dce2d-106">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="dce2d-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="dce2d-107">Наследуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dce2d-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dce2d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dce2d-108">Properties</span></span>
|<span data-ttu-id="dce2d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dce2d-109">Property</span></span>|<span data-ttu-id="dce2d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dce2d-110">Type</span></span>|<span data-ttu-id="dce2d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dce2d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dce2d-112">Хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="dce2d-112">homeButtonCustomURL</span></span>|<span data-ttu-id="dce2d-113">String</span><span class="sxs-lookup"><span data-stu-id="dce2d-113">String</span></span>|<span data-ttu-id="dce2d-114">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="dce2d-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dce2d-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="dce2d-115">Relationships</span></span>
<span data-ttu-id="dce2d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="dce2d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dce2d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dce2d-117">JSON Representation</span></span>
<span data-ttu-id="dce2d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dce2d-118">Here is a JSON representation of the resource.</span></span>
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





