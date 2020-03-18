---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ba83e4ee870a5e258a40c0c94d8d157f8564a91
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791893"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="58368-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="58368-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="58368-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58368-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58368-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58368-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58368-106">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="58368-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="58368-107">Наследуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58368-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58368-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="58368-108">Properties</span></span>
|<span data-ttu-id="58368-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="58368-109">Property</span></span>|<span data-ttu-id="58368-110">Тип</span><span class="sxs-lookup"><span data-stu-id="58368-110">Type</span></span>|<span data-ttu-id="58368-111">Описание</span><span class="sxs-lookup"><span data-stu-id="58368-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58368-112">хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="58368-112">homeButtonCustomURL</span></span>|<span data-ttu-id="58368-113">String</span><span class="sxs-lookup"><span data-stu-id="58368-113">String</span></span>|<span data-ttu-id="58368-114">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="58368-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58368-115">Связи</span><span class="sxs-lookup"><span data-stu-id="58368-115">Relationships</span></span>
<span data-ttu-id="58368-116">Нет</span><span class="sxs-lookup"><span data-stu-id="58368-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58368-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58368-117">JSON Representation</span></span>
<span data-ttu-id="58368-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58368-118">Here is a JSON representation of the resource.</span></span>
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



