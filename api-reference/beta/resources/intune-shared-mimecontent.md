---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 052cf1833d1fc7148024f6066966e4aa0a86221e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347957"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="cd7d2-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="cd7d2-103">mimeContent resource type</span></span>

> <span data-ttu-id="cd7d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd7d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd7d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd7d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd7d2-106">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="cd7d2-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="cd7d2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd7d2-107">Properties</span></span>
|<span data-ttu-id="cd7d2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd7d2-108">Property</span></span>|<span data-ttu-id="cd7d2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cd7d2-109">Type</span></span>|<span data-ttu-id="cd7d2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd7d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd7d2-111">type</span><span class="sxs-lookup"><span data-stu-id="cd7d2-111">type</span></span>|<span data-ttu-id="cd7d2-112">String</span><span class="sxs-lookup"><span data-stu-id="cd7d2-112">String</span></span>|<span data-ttu-id="cd7d2-113">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="cd7d2-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="cd7d2-114">value</span><span class="sxs-lookup"><span data-stu-id="cd7d2-114">value</span></span>|<span data-ttu-id="cd7d2-115">Binary</span><span class="sxs-lookup"><span data-stu-id="cd7d2-115">Binary</span></span>|<span data-ttu-id="cd7d2-116">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="cd7d2-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd7d2-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="cd7d2-117">Relationships</span></span>
<span data-ttu-id="cd7d2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="cd7d2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd7d2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd7d2-119">JSON Representation</span></span>
<span data-ttu-id="cd7d2-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd7d2-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



