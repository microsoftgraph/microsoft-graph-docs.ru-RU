---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
ms.openlocfilehash: 803dd9e347ef06bc9d4a9fce13d2265c4fc969a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027582"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="a0d48-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="a0d48-103">keyValuePair resource type</span></span>

> <span data-ttu-id="a0d48-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a0d48-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0d48-105">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="a0d48-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="a0d48-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0d48-106">Properties</span></span>
|<span data-ttu-id="a0d48-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0d48-107">Property</span></span>|<span data-ttu-id="a0d48-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a0d48-108">Type</span></span>|<span data-ttu-id="a0d48-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a0d48-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d48-110">name</span><span class="sxs-lookup"><span data-stu-id="a0d48-110">name</span></span>|<span data-ttu-id="a0d48-111">String</span><span class="sxs-lookup"><span data-stu-id="a0d48-111">String</span></span>|<span data-ttu-id="a0d48-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="a0d48-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="a0d48-113">value</span><span class="sxs-lookup"><span data-stu-id="a0d48-113">value</span></span>|<span data-ttu-id="a0d48-114">String</span><span class="sxs-lookup"><span data-stu-id="a0d48-114">String</span></span>|<span data-ttu-id="a0d48-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="a0d48-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0d48-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a0d48-116">Relationships</span></span>
<span data-ttu-id="a0d48-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a0d48-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0d48-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0d48-118">JSON Representation</span></span>
<span data-ttu-id="a0d48-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0d48-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



