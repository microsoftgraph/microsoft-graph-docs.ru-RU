---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f2224d255e8aa4ceb48554fdc01356277ffbc89
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939119"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="edfce-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="edfce-103">mimeContent resource type</span></span>

> <span data-ttu-id="edfce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edfce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edfce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edfce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edfce-106">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="edfce-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="edfce-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="edfce-107">Properties</span></span>
|<span data-ttu-id="edfce-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="edfce-108">Property</span></span>|<span data-ttu-id="edfce-109">Тип</span><span class="sxs-lookup"><span data-stu-id="edfce-109">Type</span></span>|<span data-ttu-id="edfce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="edfce-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edfce-111">type</span><span class="sxs-lookup"><span data-stu-id="edfce-111">type</span></span>|<span data-ttu-id="edfce-112">String</span><span class="sxs-lookup"><span data-stu-id="edfce-112">String</span></span>|<span data-ttu-id="edfce-113">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="edfce-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="edfce-114">value</span><span class="sxs-lookup"><span data-stu-id="edfce-114">value</span></span>|<span data-ttu-id="edfce-115">Binary</span><span class="sxs-lookup"><span data-stu-id="edfce-115">Binary</span></span>|<span data-ttu-id="edfce-116">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="edfce-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edfce-117">Связи</span><span class="sxs-lookup"><span data-stu-id="edfce-117">Relationships</span></span>
<span data-ttu-id="edfce-118">Нет</span><span class="sxs-lookup"><span data-stu-id="edfce-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edfce-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edfce-119">JSON Representation</span></span>
<span data-ttu-id="edfce-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edfce-120">Here is a JSON representation of the resource.</span></span>
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




