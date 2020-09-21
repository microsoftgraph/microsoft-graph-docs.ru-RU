---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 956eada9779d4da925025878a2464ceb3e9a1ad2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968411"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="b33fa-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="b33fa-103">mimeContent resource type</span></span>

<span data-ttu-id="b33fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b33fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b33fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b33fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b33fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b33fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b33fa-107">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="b33fa-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="b33fa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b33fa-108">Properties</span></span>
|<span data-ttu-id="b33fa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b33fa-109">Property</span></span>|<span data-ttu-id="b33fa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b33fa-110">Type</span></span>|<span data-ttu-id="b33fa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b33fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b33fa-112">type</span><span class="sxs-lookup"><span data-stu-id="b33fa-112">type</span></span>|<span data-ttu-id="b33fa-113">String</span><span class="sxs-lookup"><span data-stu-id="b33fa-113">String</span></span>|<span data-ttu-id="b33fa-114">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="b33fa-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="b33fa-115">value</span><span class="sxs-lookup"><span data-stu-id="b33fa-115">value</span></span>|<span data-ttu-id="b33fa-116">Binary</span><span class="sxs-lookup"><span data-stu-id="b33fa-116">Binary</span></span>|<span data-ttu-id="b33fa-117">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="b33fa-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b33fa-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b33fa-118">Relationships</span></span>
<span data-ttu-id="b33fa-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b33fa-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b33fa-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b33fa-120">JSON Representation</span></span>
<span data-ttu-id="b33fa-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b33fa-121">Here is a JSON representation of the resource.</span></span>
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






