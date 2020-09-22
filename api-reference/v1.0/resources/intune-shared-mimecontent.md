---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6517f575944f5ee4b769dcee75ba3805630f718
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028373"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="e349b-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="e349b-103">mimeContent resource type</span></span>

<span data-ttu-id="e349b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e349b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e349b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e349b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e349b-106">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="e349b-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="e349b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e349b-107">Properties</span></span>
|<span data-ttu-id="e349b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e349b-108">Property</span></span>|<span data-ttu-id="e349b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e349b-109">Type</span></span>|<span data-ttu-id="e349b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e349b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e349b-111">type</span><span class="sxs-lookup"><span data-stu-id="e349b-111">type</span></span>|<span data-ttu-id="e349b-112">String</span><span class="sxs-lookup"><span data-stu-id="e349b-112">String</span></span>|<span data-ttu-id="e349b-113">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="e349b-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="e349b-114">value</span><span class="sxs-lookup"><span data-stu-id="e349b-114">value</span></span>|<span data-ttu-id="e349b-115">Binary</span><span class="sxs-lookup"><span data-stu-id="e349b-115">Binary</span></span>|<span data-ttu-id="e349b-116">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="e349b-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e349b-117">Связи</span><span class="sxs-lookup"><span data-stu-id="e349b-117">Relationships</span></span>
<span data-ttu-id="e349b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e349b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e349b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e349b-119">JSON Representation</span></span>
<span data-ttu-id="e349b-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e349b-120">Here is a JSON representation of the resource.</span></span>
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









