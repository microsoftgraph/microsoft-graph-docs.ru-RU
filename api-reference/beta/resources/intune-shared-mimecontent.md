---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a867133dca99fb15044452163b050fdcb2f3d14
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527358"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="e995b-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="e995b-103">mimeContent resource type</span></span>

<span data-ttu-id="e995b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e995b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e995b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e995b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e995b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e995b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e995b-107">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="e995b-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="e995b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e995b-108">Properties</span></span>
|<span data-ttu-id="e995b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e995b-109">Property</span></span>|<span data-ttu-id="e995b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e995b-110">Type</span></span>|<span data-ttu-id="e995b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e995b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e995b-112">type</span><span class="sxs-lookup"><span data-stu-id="e995b-112">type</span></span>|<span data-ttu-id="e995b-113">String</span><span class="sxs-lookup"><span data-stu-id="e995b-113">String</span></span>|<span data-ttu-id="e995b-114">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="e995b-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="e995b-115">value</span><span class="sxs-lookup"><span data-stu-id="e995b-115">value</span></span>|<span data-ttu-id="e995b-116">Binary</span><span class="sxs-lookup"><span data-stu-id="e995b-116">Binary</span></span>|<span data-ttu-id="e995b-117">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="e995b-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e995b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e995b-118">Relationships</span></span>
<span data-ttu-id="e995b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e995b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e995b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e995b-120">JSON Representation</span></span>
<span data-ttu-id="e995b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e995b-121">Here is a JSON representation of the resource.</span></span>
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



