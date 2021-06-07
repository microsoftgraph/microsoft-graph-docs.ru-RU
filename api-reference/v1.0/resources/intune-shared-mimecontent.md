---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e17fd6abb6470fe46c836f7ed4b9f38362abb74d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751554"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="4f9b2-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="4f9b2-103">mimeContent resource type</span></span>

<span data-ttu-id="4f9b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f9b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f9b2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f9b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f9b2-106">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="4f9b2-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="4f9b2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f9b2-107">Properties</span></span>
|<span data-ttu-id="4f9b2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f9b2-108">Property</span></span>|<span data-ttu-id="4f9b2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4f9b2-109">Type</span></span>|<span data-ttu-id="4f9b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4f9b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f9b2-111">type</span><span class="sxs-lookup"><span data-stu-id="4f9b2-111">type</span></span>|<span data-ttu-id="4f9b2-112">String</span><span class="sxs-lookup"><span data-stu-id="4f9b2-112">String</span></span>|<span data-ttu-id="4f9b2-113">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="4f9b2-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="4f9b2-114">value</span><span class="sxs-lookup"><span data-stu-id="4f9b2-114">value</span></span>|<span data-ttu-id="4f9b2-115">Binary</span><span class="sxs-lookup"><span data-stu-id="4f9b2-115">Binary</span></span>|<span data-ttu-id="4f9b2-116">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="4f9b2-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f9b2-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="4f9b2-117">Relationships</span></span>
<span data-ttu-id="4f9b2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="4f9b2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f9b2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f9b2-119">JSON Representation</span></span>
<span data-ttu-id="4f9b2-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f9b2-120">Here is a JSON representation of the resource.</span></span>
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




