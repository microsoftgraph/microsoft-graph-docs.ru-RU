---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de4360ce5a8873fde7d3286f55fc0c8993936a7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571879"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="984d9-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="984d9-103">mimeContent resource type</span></span>

> <span data-ttu-id="984d9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="984d9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="984d9-105">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="984d9-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="984d9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="984d9-106">Properties</span></span>
|<span data-ttu-id="984d9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="984d9-107">Property</span></span>|<span data-ttu-id="984d9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="984d9-108">Type</span></span>|<span data-ttu-id="984d9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="984d9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="984d9-110">type</span><span class="sxs-lookup"><span data-stu-id="984d9-110">type</span></span>|<span data-ttu-id="984d9-111">String</span><span class="sxs-lookup"><span data-stu-id="984d9-111">String</span></span>|<span data-ttu-id="984d9-112">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="984d9-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="984d9-113">value</span><span class="sxs-lookup"><span data-stu-id="984d9-113">value</span></span>|<span data-ttu-id="984d9-114">Binary</span><span class="sxs-lookup"><span data-stu-id="984d9-114">Binary</span></span>|<span data-ttu-id="984d9-115">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="984d9-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="984d9-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="984d9-116">Relationships</span></span>
<span data-ttu-id="984d9-117">Нет</span><span class="sxs-lookup"><span data-stu-id="984d9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="984d9-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="984d9-118">JSON Representation</span></span>
<span data-ttu-id="984d9-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="984d9-119">Here is a JSON representation of the resource.</span></span>
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



