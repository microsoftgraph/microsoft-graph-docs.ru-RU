---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: bbe4faaffbf53c24d4d0f5b8ea1f5ee1e1966a2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860125"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="6b9d8-102">Тип ресурса storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="6b9d8-102">storagePlanInformation resource type</span></span>

> <span data-ttu-id="6b9d8-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b9d8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b9d8-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b9d8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b9d8-105">Ресурс **storagePlanInformation** содержит сведения о планы квоты хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="6b9d8-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="6b9d8-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b9d8-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```
## <a name="properties"></a><span data-ttu-id="6b9d8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b9d8-107">Properties</span></span>

| <span data-ttu-id="6b9d8-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6b9d8-108">Property name</span></span>     | <span data-ttu-id="6b9d8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6b9d8-109">Type</span></span>      | <span data-ttu-id="6b9d8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b9d8-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="6b9d8-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="6b9d8-111">upgradeAvailable</span></span>  | <span data-ttu-id="6b9d8-112">Логический</span><span class="sxs-lookup"><span data-stu-id="6b9d8-112">Boolean</span></span>   | <span data-ttu-id="6b9d8-113">Указывает, если доступны выше планы квота хранилища.</span><span class="sxs-lookup"><span data-stu-id="6b9d8-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="6b9d8-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b9d8-114">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

