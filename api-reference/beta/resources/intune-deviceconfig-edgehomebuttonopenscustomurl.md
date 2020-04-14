---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c3be48340552a9e3ba5a0bc8143363846465fbf1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386332"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="2021e-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="2021e-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="2021e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2021e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2021e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2021e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2021e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2021e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2021e-107">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="2021e-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="2021e-108">Наследуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2021e-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2021e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2021e-109">Properties</span></span>
|<span data-ttu-id="2021e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2021e-110">Property</span></span>|<span data-ttu-id="2021e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2021e-111">Type</span></span>|<span data-ttu-id="2021e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2021e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2021e-113">хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="2021e-113">homeButtonCustomURL</span></span>|<span data-ttu-id="2021e-114">String</span><span class="sxs-lookup"><span data-stu-id="2021e-114">String</span></span>|<span data-ttu-id="2021e-115">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="2021e-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2021e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="2021e-116">Relationships</span></span>
<span data-ttu-id="2021e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2021e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2021e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2021e-118">JSON Representation</span></span>
<span data-ttu-id="2021e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2021e-119">Here is a JSON representation of the resource.</span></span>
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



