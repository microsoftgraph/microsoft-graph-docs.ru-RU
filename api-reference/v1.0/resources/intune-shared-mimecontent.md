---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a0b63289b3d7666eb27de7e6dc4e643dd9fa4772
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857045"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="97291-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="97291-103">mimeContent resource type</span></span>

> <span data-ttu-id="97291-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="97291-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97291-105">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="97291-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="97291-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="97291-106">Properties</span></span>
|<span data-ttu-id="97291-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="97291-107">Property</span></span>|<span data-ttu-id="97291-108">Тип</span><span class="sxs-lookup"><span data-stu-id="97291-108">Type</span></span>|<span data-ttu-id="97291-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97291-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97291-110">type</span><span class="sxs-lookup"><span data-stu-id="97291-110">type</span></span>|<span data-ttu-id="97291-111">Строка</span><span class="sxs-lookup"><span data-stu-id="97291-111">String</span></span>|<span data-ttu-id="97291-112">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="97291-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="97291-113">value</span><span class="sxs-lookup"><span data-stu-id="97291-113">value</span></span>|<span data-ttu-id="97291-114">Binary</span><span class="sxs-lookup"><span data-stu-id="97291-114">Binary</span></span>|<span data-ttu-id="97291-115">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="97291-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97291-116">Связи</span><span class="sxs-lookup"><span data-stu-id="97291-116">Relationships</span></span>
<span data-ttu-id="97291-117">Нет</span><span class="sxs-lookup"><span data-stu-id="97291-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97291-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97291-118">JSON Representation</span></span>
<span data-ttu-id="97291-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97291-119">Here is a JSON representation of the resource.</span></span>
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



