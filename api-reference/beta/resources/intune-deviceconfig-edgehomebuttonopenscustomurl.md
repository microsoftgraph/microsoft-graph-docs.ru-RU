---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dad4baba5fd55b99efd6b2b7ebadf1973d6c9c8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783717"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="b72c0-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="b72c0-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="b72c0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b72c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b72c0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b72c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b72c0-106">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="b72c0-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="b72c0-107">НаСледуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b72c0-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b72c0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b72c0-108">Properties</span></span>
|<span data-ttu-id="b72c0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b72c0-109">Property</span></span>|<span data-ttu-id="b72c0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b72c0-110">Type</span></span>|<span data-ttu-id="b72c0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b72c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b72c0-112">Хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="b72c0-112">homeButtonCustomURL</span></span>|<span data-ttu-id="b72c0-113">String</span><span class="sxs-lookup"><span data-stu-id="b72c0-113">String</span></span>|<span data-ttu-id="b72c0-114">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="b72c0-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b72c0-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="b72c0-115">Relationships</span></span>
<span data-ttu-id="b72c0-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b72c0-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b72c0-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b72c0-117">JSON Representation</span></span>
<span data-ttu-id="b72c0-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b72c0-118">Here is a JSON representation of the resource.</span></span>
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





