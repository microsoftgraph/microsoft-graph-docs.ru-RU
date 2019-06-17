---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8114074b99957c687079ac80abef7a4f704444b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986377"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="01496-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="01496-103">mimeContent resource type</span></span>

> <span data-ttu-id="01496-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01496-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01496-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01496-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01496-106">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="01496-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="01496-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="01496-107">Properties</span></span>
|<span data-ttu-id="01496-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="01496-108">Property</span></span>|<span data-ttu-id="01496-109">Тип</span><span class="sxs-lookup"><span data-stu-id="01496-109">Type</span></span>|<span data-ttu-id="01496-110">Описание</span><span class="sxs-lookup"><span data-stu-id="01496-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01496-111">type</span><span class="sxs-lookup"><span data-stu-id="01496-111">type</span></span>|<span data-ttu-id="01496-112">String</span><span class="sxs-lookup"><span data-stu-id="01496-112">String</span></span>|<span data-ttu-id="01496-113">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="01496-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="01496-114">value</span><span class="sxs-lookup"><span data-stu-id="01496-114">value</span></span>|<span data-ttu-id="01496-115">Binary</span><span class="sxs-lookup"><span data-stu-id="01496-115">Binary</span></span>|<span data-ttu-id="01496-116">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="01496-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01496-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="01496-117">Relationships</span></span>
<span data-ttu-id="01496-118">Нет</span><span class="sxs-lookup"><span data-stu-id="01496-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01496-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01496-119">JSON Representation</span></span>
<span data-ttu-id="01496-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01496-120">Here is a JSON representation of the resource.</span></span>
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





