---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62132b9e55b8130f82fc8414cbb6e90ba34bb70f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413460"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="dad64-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="dad64-103">mimeContent resource type</span></span>

> <span data-ttu-id="dad64-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dad64-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dad64-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dad64-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dad64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dad64-107">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="dad64-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="dad64-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dad64-108">Properties</span></span>
|<span data-ttu-id="dad64-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dad64-109">Property</span></span>|<span data-ttu-id="dad64-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dad64-110">Type</span></span>|<span data-ttu-id="dad64-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dad64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dad64-112">type</span><span class="sxs-lookup"><span data-stu-id="dad64-112">type</span></span>|<span data-ttu-id="dad64-113">String</span><span class="sxs-lookup"><span data-stu-id="dad64-113">String</span></span>|<span data-ttu-id="dad64-114">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="dad64-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="dad64-115">value</span><span class="sxs-lookup"><span data-stu-id="dad64-115">value</span></span>|<span data-ttu-id="dad64-116">Binary</span><span class="sxs-lookup"><span data-stu-id="dad64-116">Binary</span></span>|<span data-ttu-id="dad64-117">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="dad64-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dad64-118">Связи</span><span class="sxs-lookup"><span data-stu-id="dad64-118">Relationships</span></span>
<span data-ttu-id="dad64-119">Нет</span><span class="sxs-lookup"><span data-stu-id="dad64-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dad64-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dad64-120">JSON Representation</span></span>
<span data-ttu-id="dad64-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dad64-121">Here is a JSON representation of the resource.</span></span>
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




