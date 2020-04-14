---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86537f6d93f2ff50c212105fce3f4fb91f137184
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466168"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="95973-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="95973-103">mimeContent resource type</span></span>

<span data-ttu-id="95973-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95973-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95973-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95973-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95973-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95973-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95973-107">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="95973-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="95973-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="95973-108">Properties</span></span>
|<span data-ttu-id="95973-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="95973-109">Property</span></span>|<span data-ttu-id="95973-110">Тип</span><span class="sxs-lookup"><span data-stu-id="95973-110">Type</span></span>|<span data-ttu-id="95973-111">Описание</span><span class="sxs-lookup"><span data-stu-id="95973-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95973-112">type</span><span class="sxs-lookup"><span data-stu-id="95973-112">type</span></span>|<span data-ttu-id="95973-113">String</span><span class="sxs-lookup"><span data-stu-id="95973-113">String</span></span>|<span data-ttu-id="95973-114">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="95973-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="95973-115">value</span><span class="sxs-lookup"><span data-stu-id="95973-115">value</span></span>|<span data-ttu-id="95973-116">Binary</span><span class="sxs-lookup"><span data-stu-id="95973-116">Binary</span></span>|<span data-ttu-id="95973-117">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="95973-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95973-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="95973-118">Relationships</span></span>
<span data-ttu-id="95973-119">Нет</span><span class="sxs-lookup"><span data-stu-id="95973-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95973-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95973-120">JSON Representation</span></span>
<span data-ttu-id="95973-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95973-121">Here is a JSON representation of the resource.</span></span>
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



