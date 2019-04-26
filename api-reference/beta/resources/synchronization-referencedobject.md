---
title: Тип ресурса Референцедобжект
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
ms.openlocfilehash: 185691c970a5555d23b7b349cef546fb85be0893
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345609"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="db55a-103">Тип ресурса Референцедобжект</span><span class="sxs-lookup"><span data-stu-id="db55a-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db55a-104">Описывает ссылку на другой объект, определенный в том же [определении каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="db55a-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="db55a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="db55a-105">Properties</span></span>

| <span data-ttu-id="db55a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="db55a-106">Property</span></span>                   | <span data-ttu-id="db55a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="db55a-107">Type</span></span>                      | <span data-ttu-id="db55a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="db55a-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="db55a-109">Референцедобжектнаме</span><span class="sxs-lookup"><span data-stu-id="db55a-109">referencedObjectName</span></span>        |<span data-ttu-id="db55a-110">String</span><span class="sxs-lookup"><span data-stu-id="db55a-110">String</span></span>                     |<span data-ttu-id="db55a-111">Имя объекта, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="db55a-111">Name of the referenced object.</span></span> <span data-ttu-id="db55a-112">Должен сопоставлять один из объектов в [определении каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="db55a-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="db55a-113">Референцедпроперти</span><span class="sxs-lookup"><span data-stu-id="db55a-113">referencedProperty</span></span>          |<span data-ttu-id="db55a-114">String</span><span class="sxs-lookup"><span data-stu-id="db55a-114">String</span></span>                     |<span data-ttu-id="db55a-115">**В настоящее время не поддерживается**.</span><span class="sxs-lookup"><span data-stu-id="db55a-115">**Currently not supported**.</span></span> <span data-ttu-id="db55a-116">Имя свойства в объекте, на который указывает ссылка, значение, которое используется в качестве ссылки.</span><span class="sxs-lookup"><span data-stu-id="db55a-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db55a-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="db55a-117">JSON representation</span></span>

<span data-ttu-id="db55a-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db55a-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
            
