---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24563bb89af91c05dd71aeb284934c0406819711
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036892"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="f5e35-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="f5e35-103">mimeContent resource type</span></span>

> <span data-ttu-id="f5e35-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5e35-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5e35-105">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="f5e35-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="f5e35-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5e35-106">Properties</span></span>
|<span data-ttu-id="f5e35-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5e35-107">Property</span></span>|<span data-ttu-id="f5e35-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f5e35-108">Type</span></span>|<span data-ttu-id="f5e35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f5e35-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5e35-110">type</span><span class="sxs-lookup"><span data-stu-id="f5e35-110">type</span></span>|<span data-ttu-id="f5e35-111">String</span><span class="sxs-lookup"><span data-stu-id="f5e35-111">String</span></span>|<span data-ttu-id="f5e35-112">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="f5e35-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="f5e35-113">value</span><span class="sxs-lookup"><span data-stu-id="f5e35-113">value</span></span>|<span data-ttu-id="f5e35-114">Binary</span><span class="sxs-lookup"><span data-stu-id="f5e35-114">Binary</span></span>|<span data-ttu-id="f5e35-115">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="f5e35-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5e35-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="f5e35-116">Relationships</span></span>
<span data-ttu-id="f5e35-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f5e35-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5e35-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5e35-118">JSON Representation</span></span>
<span data-ttu-id="f5e35-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5e35-119">Here is a JSON representation of the resource.</span></span>
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



