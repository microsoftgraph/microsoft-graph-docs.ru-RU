---
author: learafa
description: Ресурс storagePlanInformation предоставляет сведения о планах квот хранилища диска.
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: b8b4778a4726c227bfe79ad13ecb14507b13a889
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036956"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="de0be-103">Тип ресурса storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="de0be-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="de0be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de0be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de0be-105">Предоставляет сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="de0be-105">Provides information about the drive's storage quota plans.</span></span>

## <a name="properties"></a><span data-ttu-id="de0be-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="de0be-106">Properties</span></span>

| <span data-ttu-id="de0be-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="de0be-107">Property name</span></span>     | <span data-ttu-id="de0be-108">Тип</span><span class="sxs-lookup"><span data-stu-id="de0be-108">Type</span></span>      | <span data-ttu-id="de0be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="de0be-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="de0be-110">**упградеаваилабле**</span><span class="sxs-lookup"><span data-stu-id="de0be-110">**upgradeAvailable**</span></span>  | <span data-ttu-id="de0be-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0be-111">Boolean</span></span>   | <span data-ttu-id="de0be-112">Указывает, доступны ли планы квоты для хранилища выше.</span><span class="sxs-lookup"><span data-stu-id="de0be-112">Indicates whether there are higher storage quota plans available.</span></span> <span data-ttu-id="de0be-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="de0be-113">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="de0be-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de0be-114">JSON representation</span></span>

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


