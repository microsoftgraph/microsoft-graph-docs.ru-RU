---
title: Тип ресурса referencedObject
description: Описывает ссылку на другой объект, определенных в одно и то же определение каталога.
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529322"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="e658b-103">Тип ресурса referencedObject</span><span class="sxs-lookup"><span data-stu-id="e658b-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e658b-104">Описывает ссылку на другой объект, определенных в одно и то же [Определение каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e658b-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e658b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e658b-105">Properties</span></span>

| <span data-ttu-id="e658b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e658b-106">Property</span></span>                   | <span data-ttu-id="e658b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e658b-107">Type</span></span>                      | <span data-ttu-id="e658b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e658b-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="e658b-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="e658b-109">referencedObjectName</span></span>        |<span data-ttu-id="e658b-110">String</span><span class="sxs-lookup"><span data-stu-id="e658b-110">String</span></span>                     |<span data-ttu-id="e658b-111">Имя объекта, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="e658b-111">Name of the referenced object.</span></span> <span data-ttu-id="e658b-112">Должно соответствовать одному из объектов в [каталоге определения](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e658b-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="e658b-113">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="e658b-113">referencedProperty</span></span>          |<span data-ttu-id="e658b-114">String</span><span class="sxs-lookup"><span data-stu-id="e658b-114">String</span></span>                     |<span data-ttu-id="e658b-115">**В настоящее время не поддерживается**.</span><span class="sxs-lookup"><span data-stu-id="e658b-115">**Currently not supported**.</span></span> <span data-ttu-id="e658b-116">Имя свойства в этом объекте, значение которой используется в качестве ссылки.</span><span class="sxs-lookup"><span data-stu-id="e658b-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e658b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e658b-117">JSON representation</span></span>

<span data-ttu-id="e658b-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e658b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-referencedobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
            
