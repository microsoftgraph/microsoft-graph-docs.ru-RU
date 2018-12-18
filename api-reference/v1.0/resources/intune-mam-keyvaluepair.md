---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
ms.openlocfilehash: 078d414330e7a6c333042b6f6eb83ec44e255d73
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355082"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="9fc5f-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="9fc5f-103">keyValuePair resource type</span></span>

> <span data-ttu-id="9fc5f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9fc5f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fc5f-105">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="9fc5f-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="9fc5f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fc5f-106">Properties</span></span>
|<span data-ttu-id="9fc5f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fc5f-107">Property</span></span>|<span data-ttu-id="9fc5f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9fc5f-108">Type</span></span>|<span data-ttu-id="9fc5f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc5f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fc5f-110">name</span><span class="sxs-lookup"><span data-stu-id="9fc5f-110">name</span></span>|<span data-ttu-id="9fc5f-111">Строка</span><span class="sxs-lookup"><span data-stu-id="9fc5f-111">String</span></span>|<span data-ttu-id="9fc5f-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="9fc5f-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="9fc5f-113">value</span><span class="sxs-lookup"><span data-stu-id="9fc5f-113">value</span></span>|<span data-ttu-id="9fc5f-114">Строка</span><span class="sxs-lookup"><span data-stu-id="9fc5f-114">String</span></span>|<span data-ttu-id="9fc5f-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="9fc5f-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fc5f-116">Связи</span><span class="sxs-lookup"><span data-stu-id="9fc5f-116">Relationships</span></span>
<span data-ttu-id="9fc5f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9fc5f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9fc5f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fc5f-118">JSON Representation</span></span>
<span data-ttu-id="9fc5f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fc5f-119">Here is a JSON representation of the resource.</span></span>
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



