---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
ms.openlocfilehash: cc0d024c814588479e641114ad33d19a5e609ecd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080528"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="a9f53-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="a9f53-103">mimeContent resource type</span></span>

> <span data-ttu-id="a9f53-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9f53-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9f53-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9f53-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a9f53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9f53-107">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="a9f53-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="a9f53-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9f53-108">Properties</span></span>
|<span data-ttu-id="a9f53-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9f53-109">Property</span></span>|<span data-ttu-id="a9f53-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a9f53-110">Type</span></span>|<span data-ttu-id="a9f53-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a9f53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f53-112">type</span><span class="sxs-lookup"><span data-stu-id="a9f53-112">type</span></span>|<span data-ttu-id="a9f53-113">String</span><span class="sxs-lookup"><span data-stu-id="a9f53-113">String</span></span>|<span data-ttu-id="a9f53-114">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="a9f53-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="a9f53-115">value</span><span class="sxs-lookup"><span data-stu-id="a9f53-115">value</span></span>|<span data-ttu-id="a9f53-116">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a9f53-116">Binary</span></span>|<span data-ttu-id="a9f53-117">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="a9f53-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9f53-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a9f53-118">Relationships</span></span>
<span data-ttu-id="a9f53-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a9f53-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9f53-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9f53-120">JSON Representation</span></span>
<span data-ttu-id="a9f53-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9f53-121">Here is a JSON representation of the resource.</span></span>
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





