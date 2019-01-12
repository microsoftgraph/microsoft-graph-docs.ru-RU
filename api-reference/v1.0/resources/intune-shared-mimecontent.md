---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a486753c95afce9dff6ceec5846ff618b9103b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971902"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="53f2f-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="53f2f-103">mimeContent resource type</span></span>

> <span data-ttu-id="53f2f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="53f2f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53f2f-105">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="53f2f-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="53f2f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="53f2f-106">Properties</span></span>
|<span data-ttu-id="53f2f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="53f2f-107">Property</span></span>|<span data-ttu-id="53f2f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="53f2f-108">Type</span></span>|<span data-ttu-id="53f2f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="53f2f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53f2f-110">type</span><span class="sxs-lookup"><span data-stu-id="53f2f-110">type</span></span>|<span data-ttu-id="53f2f-111">Строка</span><span class="sxs-lookup"><span data-stu-id="53f2f-111">String</span></span>|<span data-ttu-id="53f2f-112">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="53f2f-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="53f2f-113">value</span><span class="sxs-lookup"><span data-stu-id="53f2f-113">value</span></span>|<span data-ttu-id="53f2f-114">Binary</span><span class="sxs-lookup"><span data-stu-id="53f2f-114">Binary</span></span>|<span data-ttu-id="53f2f-115">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="53f2f-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53f2f-116">Связи</span><span class="sxs-lookup"><span data-stu-id="53f2f-116">Relationships</span></span>
<span data-ttu-id="53f2f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="53f2f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="53f2f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53f2f-118">JSON Representation</span></span>
<span data-ttu-id="53f2f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53f2f-119">Here is a JSON representation of the resource.</span></span>
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



