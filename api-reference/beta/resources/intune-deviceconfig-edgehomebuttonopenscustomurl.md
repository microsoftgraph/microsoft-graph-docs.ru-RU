---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b82acaf8ef5f6e008d759f257c7382ff64492b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946821"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="d8033-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="d8033-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="d8033-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8033-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8033-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8033-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8033-106">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="d8033-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="d8033-107">Наследуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8033-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d8033-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8033-108">Properties</span></span>
|<span data-ttu-id="d8033-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8033-109">Property</span></span>|<span data-ttu-id="d8033-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d8033-110">Type</span></span>|<span data-ttu-id="d8033-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8033-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8033-112">Хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="d8033-112">homeButtonCustomURL</span></span>|<span data-ttu-id="d8033-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d8033-113">String</span></span>|<span data-ttu-id="d8033-114">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="d8033-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8033-115">Связи</span><span class="sxs-lookup"><span data-stu-id="d8033-115">Relationships</span></span>
<span data-ttu-id="d8033-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d8033-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8033-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8033-117">JSON Representation</span></span>
<span data-ttu-id="d8033-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8033-118">Here is a JSON representation of the resource.</span></span>
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




