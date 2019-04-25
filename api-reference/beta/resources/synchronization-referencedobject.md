---
title: Тип ресурса Референцедобжект
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523247"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="efd99-103">Тип ресурса Референцедобжект</span><span class="sxs-lookup"><span data-stu-id="efd99-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd99-104">Описывает ссылку на другой объект, определенный в том же [определении каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="efd99-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="efd99-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="efd99-105">Properties</span></span>

| <span data-ttu-id="efd99-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="efd99-106">Property</span></span>                   | <span data-ttu-id="efd99-107">Тип</span><span class="sxs-lookup"><span data-stu-id="efd99-107">Type</span></span>                      | <span data-ttu-id="efd99-108">Описание</span><span class="sxs-lookup"><span data-stu-id="efd99-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="efd99-109">Референцедобжектнаме</span><span class="sxs-lookup"><span data-stu-id="efd99-109">referencedObjectName</span></span>        |<span data-ttu-id="efd99-110">String</span><span class="sxs-lookup"><span data-stu-id="efd99-110">String</span></span>                     |<span data-ttu-id="efd99-111">Имя объекта, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="efd99-111">Name of the referenced object.</span></span> <span data-ttu-id="efd99-112">Должен сопоставлять один из объектов в [определении каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="efd99-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="efd99-113">Референцедпроперти</span><span class="sxs-lookup"><span data-stu-id="efd99-113">referencedProperty</span></span>          |<span data-ttu-id="efd99-114">String</span><span class="sxs-lookup"><span data-stu-id="efd99-114">String</span></span>                     |<span data-ttu-id="efd99-115">**В настоящее время не поддерживается**.</span><span class="sxs-lookup"><span data-stu-id="efd99-115">**Currently not supported**.</span></span> <span data-ttu-id="efd99-116">Имя свойства в объекте, на который указывает ссылка, значение, которое используется в качестве ссылки.</span><span class="sxs-lookup"><span data-stu-id="efd99-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efd99-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efd99-117">JSON representation</span></span>

<span data-ttu-id="efd99-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efd99-118">The following is a JSON representation of the resource.</span></span>

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
            
