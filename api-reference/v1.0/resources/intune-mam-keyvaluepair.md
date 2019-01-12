---
title: Тип ресурса keyValuePair
description: Пара "ключ-значение" для хранения пользовательских настроек
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db3e24c1c14cb208be66b7a2b0364ad12b162956
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926444"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="180f4-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="180f4-103">keyValuePair resource type</span></span>

> <span data-ttu-id="180f4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="180f4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="180f4-105">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="180f4-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="180f4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="180f4-106">Properties</span></span>
|<span data-ttu-id="180f4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="180f4-107">Property</span></span>|<span data-ttu-id="180f4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="180f4-108">Type</span></span>|<span data-ttu-id="180f4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="180f4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="180f4-110">name</span><span class="sxs-lookup"><span data-stu-id="180f4-110">name</span></span>|<span data-ttu-id="180f4-111">Строка</span><span class="sxs-lookup"><span data-stu-id="180f4-111">String</span></span>|<span data-ttu-id="180f4-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="180f4-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="180f4-113">value</span><span class="sxs-lookup"><span data-stu-id="180f4-113">value</span></span>|<span data-ttu-id="180f4-114">Строка</span><span class="sxs-lookup"><span data-stu-id="180f4-114">String</span></span>|<span data-ttu-id="180f4-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="180f4-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="180f4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="180f4-116">Relationships</span></span>
<span data-ttu-id="180f4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="180f4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="180f4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="180f4-118">JSON Representation</span></span>
<span data-ttu-id="180f4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="180f4-119">Here is a JSON representation of the resource.</span></span>
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



