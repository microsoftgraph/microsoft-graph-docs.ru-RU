---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
ms.openlocfilehash: 7f25a1c16b86a45886cd763c1a8a3aa6142c47e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026008"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="6fbca-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="6fbca-103">mimeContent resource type</span></span>

> <span data-ttu-id="6fbca-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6fbca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fbca-105">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="6fbca-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="6fbca-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fbca-106">Properties</span></span>
|<span data-ttu-id="6fbca-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fbca-107">Property</span></span>|<span data-ttu-id="6fbca-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6fbca-108">Type</span></span>|<span data-ttu-id="6fbca-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6fbca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fbca-110">type</span><span class="sxs-lookup"><span data-stu-id="6fbca-110">type</span></span>|<span data-ttu-id="6fbca-111">String</span><span class="sxs-lookup"><span data-stu-id="6fbca-111">String</span></span>|<span data-ttu-id="6fbca-112">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="6fbca-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="6fbca-113">value</span><span class="sxs-lookup"><span data-stu-id="6fbca-113">value</span></span>|<span data-ttu-id="6fbca-114">Двоичный</span><span class="sxs-lookup"><span data-stu-id="6fbca-114">Binary</span></span>|<span data-ttu-id="6fbca-115">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="6fbca-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fbca-116">Связи</span><span class="sxs-lookup"><span data-stu-id="6fbca-116">Relationships</span></span>
<span data-ttu-id="6fbca-117">Нет</span><span class="sxs-lookup"><span data-stu-id="6fbca-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6fbca-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fbca-118">JSON Representation</span></span>
<span data-ttu-id="6fbca-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fbca-119">Here is a JSON representation of the resource.</span></span>
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



