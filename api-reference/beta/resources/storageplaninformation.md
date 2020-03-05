---
author: psampath
description: Ресурс storagePlanInformation предоставляет сведения о планах квот хранилища диска.
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 79254efa033528bd8fd4cf66a07959a71e3fef1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520438"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="b5775-103">Тип ресурса storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="b5775-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="b5775-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b5775-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5775-105">Ресурс **storagePlanInformation** предоставляет сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="b5775-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="b5775-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5775-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="b5775-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5775-107">Properties</span></span>

| <span data-ttu-id="b5775-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b5775-108">Property name</span></span>     | <span data-ttu-id="b5775-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b5775-109">Type</span></span>      | <span data-ttu-id="b5775-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b5775-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="b5775-111">упградеаваилабле</span><span class="sxs-lookup"><span data-stu-id="b5775-111">upgradeAvailable</span></span>  | <span data-ttu-id="b5775-112">Логический</span><span class="sxs-lookup"><span data-stu-id="b5775-112">Boolean</span></span>   | <span data-ttu-id="b5775-113">Указывает, доступны ли планы квоты хранилища выше.</span><span class="sxs-lookup"><span data-stu-id="b5775-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="b5775-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5775-114">Read-only.</span></span> |


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

