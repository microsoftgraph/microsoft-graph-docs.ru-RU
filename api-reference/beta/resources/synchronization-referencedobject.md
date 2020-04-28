---
title: Тип ресурса Референцедобжект
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7779fb851812c00c15749877517b79273752ab58
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217593"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="03ecb-103">Тип ресурса Референцедобжект</span><span class="sxs-lookup"><span data-stu-id="03ecb-103">referencedObject resource type</span></span>

<span data-ttu-id="03ecb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03ecb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03ecb-105">Описывает ссылку на другой объект, определенный в том же [определении каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="03ecb-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="03ecb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="03ecb-106">Properties</span></span>

| <span data-ttu-id="03ecb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="03ecb-107">Property</span></span>                   | <span data-ttu-id="03ecb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="03ecb-108">Type</span></span>                      | <span data-ttu-id="03ecb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="03ecb-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="03ecb-110">референцедобжектнаме</span><span class="sxs-lookup"><span data-stu-id="03ecb-110">referencedObjectName</span></span>        |<span data-ttu-id="03ecb-111">String</span><span class="sxs-lookup"><span data-stu-id="03ecb-111">String</span></span>                     |<span data-ttu-id="03ecb-112">Имя объекта, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="03ecb-112">Name of the referenced object.</span></span> <span data-ttu-id="03ecb-113">Должен сопоставлять один из объектов в [определении каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="03ecb-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="03ecb-114">референцедпроперти</span><span class="sxs-lookup"><span data-stu-id="03ecb-114">referencedProperty</span></span>          |<span data-ttu-id="03ecb-115">String</span><span class="sxs-lookup"><span data-stu-id="03ecb-115">String</span></span>                     |<span data-ttu-id="03ecb-116">**В настоящее время не поддерживается**.</span><span class="sxs-lookup"><span data-stu-id="03ecb-116">**Currently not supported**.</span></span> <span data-ttu-id="03ecb-117">Имя свойства в объекте, на который указывает ссылка, значение, которое используется в качестве ссылки.</span><span class="sxs-lookup"><span data-stu-id="03ecb-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03ecb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03ecb-118">JSON representation</span></span>

<span data-ttu-id="03ecb-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03ecb-119">The following is a JSON representation of the resource.</span></span>

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
            
