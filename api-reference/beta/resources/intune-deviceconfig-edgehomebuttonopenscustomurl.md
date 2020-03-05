---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60184022f219eba09f205121721b48fd6675d8c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530064"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="3b3ed-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="3b3ed-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="3b3ed-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b3ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b3ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b3ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b3ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b3ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b3ed-107">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="3b3ed-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="3b3ed-108">Наследуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b3ed-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b3ed-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b3ed-109">Properties</span></span>
|<span data-ttu-id="3b3ed-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b3ed-110">Property</span></span>|<span data-ttu-id="3b3ed-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3b3ed-111">Type</span></span>|<span data-ttu-id="3b3ed-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3b3ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b3ed-113">хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="3b3ed-113">homeButtonCustomURL</span></span>|<span data-ttu-id="3b3ed-114">String</span><span class="sxs-lookup"><span data-stu-id="3b3ed-114">String</span></span>|<span data-ttu-id="3b3ed-115">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="3b3ed-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b3ed-116">Связи</span><span class="sxs-lookup"><span data-stu-id="3b3ed-116">Relationships</span></span>
<span data-ttu-id="3b3ed-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3b3ed-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b3ed-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b3ed-118">JSON Representation</span></span>
<span data-ttu-id="3b3ed-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b3ed-119">Here is a JSON representation of the resource.</span></span>
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



