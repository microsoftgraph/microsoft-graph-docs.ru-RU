---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: 3911d3af5f2149d1043ed246e7c11d287c840842
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342961"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="75b64-102">Тип ресурса storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="75b64-102">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75b64-103">Ресурс **storagePlanInformation** предоставляет сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="75b64-103">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="75b64-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75b64-104">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="75b64-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="75b64-105">Properties</span></span>

| <span data-ttu-id="75b64-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="75b64-106">Property name</span></span>     | <span data-ttu-id="75b64-107">Тип</span><span class="sxs-lookup"><span data-stu-id="75b64-107">Type</span></span>      | <span data-ttu-id="75b64-108">Описание</span><span class="sxs-lookup"><span data-stu-id="75b64-108">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="75b64-109">Упградеаваилабле</span><span class="sxs-lookup"><span data-stu-id="75b64-109">upgradeAvailable</span></span>  | <span data-ttu-id="75b64-110">Логический</span><span class="sxs-lookup"><span data-stu-id="75b64-110">Boolean</span></span>   | <span data-ttu-id="75b64-111">Указывает, доступны ли планы квоты хранилища выше.</span><span class="sxs-lookup"><span data-stu-id="75b64-111">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="75b64-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75b64-112">Read-only.</span></span> |


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

