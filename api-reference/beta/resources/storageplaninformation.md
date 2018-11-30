---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
ms.openlocfilehash: 07552f405ec8c5d6ae8345a8238cd8aec3763b11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079817"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="a2942-102">Тип ресурса storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="a2942-102">storagePlanInformation resource type</span></span>

> <span data-ttu-id="a2942-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2942-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2942-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2942-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2942-105">Ресурс **storagePlanInformation** содержит сведения о планы квоты хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="a2942-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="a2942-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2942-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="a2942-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2942-107">Properties</span></span>

| <span data-ttu-id="a2942-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a2942-108">Property name</span></span>     | <span data-ttu-id="a2942-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a2942-109">Type</span></span>      | <span data-ttu-id="a2942-110">Description</span><span class="sxs-lookup"><span data-stu-id="a2942-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="a2942-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="a2942-111">upgradeAvailable</span></span>  | <span data-ttu-id="a2942-112">Логический</span><span class="sxs-lookup"><span data-stu-id="a2942-112">Boolean</span></span>   | <span data-ttu-id="a2942-113">Указывает, если доступны выше планы квота хранилища.</span><span class="sxs-lookup"><span data-stu-id="a2942-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="a2942-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2942-114">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

