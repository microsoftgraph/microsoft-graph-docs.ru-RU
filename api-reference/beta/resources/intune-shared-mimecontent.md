---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad580548e3f399a3c35d4f86e23eaab4dfa62979
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521266"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="dea33-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="dea33-103">mimeContent resource type</span></span>

> <span data-ttu-id="dea33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dea33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dea33-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dea33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dea33-106">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="dea33-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="dea33-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dea33-107">Properties</span></span>
|<span data-ttu-id="dea33-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dea33-108">Property</span></span>|<span data-ttu-id="dea33-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dea33-109">Type</span></span>|<span data-ttu-id="dea33-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dea33-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dea33-111">type</span><span class="sxs-lookup"><span data-stu-id="dea33-111">type</span></span>|<span data-ttu-id="dea33-112">String</span><span class="sxs-lookup"><span data-stu-id="dea33-112">String</span></span>|<span data-ttu-id="dea33-113">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="dea33-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="dea33-114">value</span><span class="sxs-lookup"><span data-stu-id="dea33-114">value</span></span>|<span data-ttu-id="dea33-115">Binary</span><span class="sxs-lookup"><span data-stu-id="dea33-115">Binary</span></span>|<span data-ttu-id="dea33-116">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="dea33-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dea33-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="dea33-117">Relationships</span></span>
<span data-ttu-id="dea33-118">Нет</span><span class="sxs-lookup"><span data-stu-id="dea33-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dea33-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dea33-119">JSON Representation</span></span>
<span data-ttu-id="dea33-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dea33-120">Here is a JSON representation of the resource.</span></span>
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





