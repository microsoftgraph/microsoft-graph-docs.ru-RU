---
title: тип ресурса featureUpdateReference
description: Представляет Windows 10 обновления функций.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 69eda05a94982429035999bd914c6f0c9847fa67
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067585"
---
# <a name="featureupdatereference-resource-type"></a><span data-ttu-id="6ddf9-103">тип ресурса featureUpdateReference</span><span class="sxs-lookup"><span data-stu-id="6ddf9-103">featureUpdateReference resource type</span></span>

<span data-ttu-id="6ddf9-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="6ddf9-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ddf9-105">Представляет Windows 10 обновления функций.</span><span class="sxs-lookup"><span data-stu-id="6ddf9-105">Represents Windows 10 feature update content.</span></span>

<span data-ttu-id="6ddf9-106">В развертывании одна и та же ссылка на обновление функций может привести к тому, что устройства получают различные изменения обновления, но содержимое считается контекстуальным эквивалентом для всех устройств в развертывании.</span><span class="sxs-lookup"><span data-stu-id="6ddf9-106">In a deployment, the same feature update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="6ddf9-107">Наследует [от windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="6ddf9-107">Inherits from [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6ddf9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ddf9-108">Properties</span></span>
|<span data-ttu-id="6ddf9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ddf9-109">Property</span></span>|<span data-ttu-id="6ddf9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6ddf9-110">Type</span></span>|<span data-ttu-id="6ddf9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6ddf9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ddf9-112">version</span><span class="sxs-lookup"><span data-stu-id="6ddf9-112">version</span></span>|<span data-ttu-id="6ddf9-113">String</span><span class="sxs-lookup"><span data-stu-id="6ddf9-113">String</span></span>|<span data-ttu-id="6ddf9-114">Указывает обновление функций по версии.</span><span class="sxs-lookup"><span data-stu-id="6ddf9-114">Specifies a feature update by version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ddf9-115">Связи</span><span class="sxs-lookup"><span data-stu-id="6ddf9-115">Relationships</span></span>
<span data-ttu-id="6ddf9-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6ddf9-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ddf9-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6ddf9-117">JSON representation</span></span>
<span data-ttu-id="6ddf9-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ddf9-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateReference",
  "version": "String"
}
```

