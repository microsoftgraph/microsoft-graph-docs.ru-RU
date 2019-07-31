---
author: psampath
description: Ресурс storagePlanInformation предоставляет сведения о планах квот хранилища диска.
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d8ddb39f9f7c6443f0e669052084af27b8fd5cec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008084"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="db902-103">Тип ресурса storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="db902-103">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db902-104">Ресурс **storagePlanInformation** предоставляет сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="db902-104">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="db902-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db902-105">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="db902-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="db902-106">Properties</span></span>

| <span data-ttu-id="db902-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="db902-107">Property name</span></span>     | <span data-ttu-id="db902-108">Тип</span><span class="sxs-lookup"><span data-stu-id="db902-108">Type</span></span>      | <span data-ttu-id="db902-109">Описание</span><span class="sxs-lookup"><span data-stu-id="db902-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="db902-110">Упградеаваилабле</span><span class="sxs-lookup"><span data-stu-id="db902-110">upgradeAvailable</span></span>  | <span data-ttu-id="db902-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="db902-111">Boolean</span></span>   | <span data-ttu-id="db902-112">Указывает, доступны ли планы квоты хранилища выше.</span><span class="sxs-lookup"><span data-stu-id="db902-112">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="db902-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db902-113">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": []
}
-->

