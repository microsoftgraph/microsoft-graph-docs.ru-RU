---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6fc230ab7644724ca971639c98394ebc256c1194
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768921"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="74120-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="74120-103">mimeContent resource type</span></span>

> <span data-ttu-id="74120-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74120-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74120-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74120-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74120-106">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="74120-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="74120-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="74120-107">Properties</span></span>
|<span data-ttu-id="74120-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="74120-108">Property</span></span>|<span data-ttu-id="74120-109">Тип</span><span class="sxs-lookup"><span data-stu-id="74120-109">Type</span></span>|<span data-ttu-id="74120-110">Описание</span><span class="sxs-lookup"><span data-stu-id="74120-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74120-111">type</span><span class="sxs-lookup"><span data-stu-id="74120-111">type</span></span>|<span data-ttu-id="74120-112">String</span><span class="sxs-lookup"><span data-stu-id="74120-112">String</span></span>|<span data-ttu-id="74120-113">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="74120-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="74120-114">value</span><span class="sxs-lookup"><span data-stu-id="74120-114">value</span></span>|<span data-ttu-id="74120-115">Binary</span><span class="sxs-lookup"><span data-stu-id="74120-115">Binary</span></span>|<span data-ttu-id="74120-116">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="74120-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74120-117">Связи</span><span class="sxs-lookup"><span data-stu-id="74120-117">Relationships</span></span>
<span data-ttu-id="74120-118">Нет</span><span class="sxs-lookup"><span data-stu-id="74120-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74120-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74120-119">JSON Representation</span></span>
<span data-ttu-id="74120-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74120-120">Here is a JSON representation of the resource.</span></span>
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



