---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b300f3d0db3a2a310d0a19408750b1dd9ac5c46
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368550"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="ac597-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="ac597-103">numberRange resource type</span></span>

> <span data-ttu-id="ac597-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac597-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac597-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac597-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac597-106">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="ac597-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="ac597-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac597-107">Properties</span></span>
|<span data-ttu-id="ac597-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac597-108">Property</span></span>|<span data-ttu-id="ac597-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ac597-109">Type</span></span>|<span data-ttu-id="ac597-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ac597-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac597-111">ловернумбер</span><span class="sxs-lookup"><span data-stu-id="ac597-111">lowerNumber</span></span>|<span data-ttu-id="ac597-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ac597-112">Int32</span></span>|<span data-ttu-id="ac597-113">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="ac597-113">Lower number.</span></span>|
|<span data-ttu-id="ac597-114">уппернумбер</span><span class="sxs-lookup"><span data-stu-id="ac597-114">upperNumber</span></span>|<span data-ttu-id="ac597-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ac597-115">Int32</span></span>|<span data-ttu-id="ac597-116">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="ac597-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac597-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="ac597-117">Relationships</span></span>
<span data-ttu-id="ac597-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ac597-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac597-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac597-119">JSON Representation</span></span>
<span data-ttu-id="ac597-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac597-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```



