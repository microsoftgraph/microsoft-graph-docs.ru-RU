---
title: Тип ресурса Синчронизатионеррор
description: Представляет сообщение об ошибке, возникшей во время процесса синхронизации.
localization_priority: Normal
ms.openlocfilehash: f37dca5b65a67eb36b2b6a130eee8feb692cd271
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525980"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="4e92c-103">Тип ресурса Синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="4e92c-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e92c-104">Представляет сообщение об ошибке, возникшей во время процесса синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4e92c-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="4e92c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e92c-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="4e92c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e92c-106">Property</span></span>     | <span data-ttu-id="4e92c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4e92c-107">Type</span></span>   |<span data-ttu-id="4e92c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4e92c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e92c-109">code</span><span class="sxs-lookup"><span data-stu-id="4e92c-109">code</span></span>|<span data-ttu-id="4e92c-110">String</span><span class="sxs-lookup"><span data-stu-id="4e92c-110">String</span></span>||
|<span data-ttu-id="4e92c-111">message</span><span class="sxs-lookup"><span data-stu-id="4e92c-111">message</span></span>|<span data-ttu-id="4e92c-112">String</span><span class="sxs-lookup"><span data-stu-id="4e92c-112">String</span></span>||
|<span data-ttu-id="4e92c-113">Тенантактионабле</span><span class="sxs-lookup"><span data-stu-id="4e92c-113">tenantActionable</span></span>|<span data-ttu-id="4e92c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e92c-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="4e92c-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4e92c-115">JSON representation</span></span>

<span data-ttu-id="4e92c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e92c-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
