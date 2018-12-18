---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
ms.openlocfilehash: 05088fa472c8f8a71adabbb0c807e7b2f0b80b09
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333497"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="c1717-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="c1717-103">mimeContent resource type</span></span>

> <span data-ttu-id="c1717-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1717-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1717-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1717-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1717-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c1717-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1717-107">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="c1717-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="c1717-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1717-108">Properties</span></span>
|<span data-ttu-id="c1717-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1717-109">Property</span></span>|<span data-ttu-id="c1717-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c1717-110">Type</span></span>|<span data-ttu-id="c1717-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1717-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1717-112">type</span><span class="sxs-lookup"><span data-stu-id="c1717-112">type</span></span>|<span data-ttu-id="c1717-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c1717-113">String</span></span>|<span data-ttu-id="c1717-114">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="c1717-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="c1717-115">value</span><span class="sxs-lookup"><span data-stu-id="c1717-115">value</span></span>|<span data-ttu-id="c1717-116">Binary</span><span class="sxs-lookup"><span data-stu-id="c1717-116">Binary</span></span>|<span data-ttu-id="c1717-117">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="c1717-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1717-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c1717-118">Relationships</span></span>
<span data-ttu-id="c1717-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c1717-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1717-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1717-120">JSON Representation</span></span>
<span data-ttu-id="c1717-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1717-121">Here is a JSON representation of the resource.</span></span>
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





