---
author: learafa
description: Ресурс storagePlanInformation предоставляет сведения о планах квот хранилища диска.
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a5e6c10bdbc8a68230a223501844d0ee121014c2
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863777"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="7f3b9-103">Тип ресурса storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="7f3b9-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="7f3b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f3b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f3b9-105">Предоставляет сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="7f3b9-105">Provides information about the drive's storage quota plans.</span></span>

## <a name="properties"></a><span data-ttu-id="7f3b9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f3b9-106">Properties</span></span>

| <span data-ttu-id="7f3b9-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7f3b9-107">Property name</span></span>     | <span data-ttu-id="7f3b9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7f3b9-108">Type</span></span>      | <span data-ttu-id="7f3b9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7f3b9-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="7f3b9-110">**упградеаваилабле**</span><span class="sxs-lookup"><span data-stu-id="7f3b9-110">**upgradeAvailable**</span></span>  | <span data-ttu-id="7f3b9-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3b9-111">Boolean</span></span>   | <span data-ttu-id="7f3b9-112">Указывает, доступны ли планы квоты для хранилища выше.</span><span class="sxs-lookup"><span data-stu-id="7f3b9-112">Indicates whether there are higher storage quota plans available.</span></span> <span data-ttu-id="7f3b9-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f3b9-113">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7f3b9-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f3b9-114">JSON representation</span></span>

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

