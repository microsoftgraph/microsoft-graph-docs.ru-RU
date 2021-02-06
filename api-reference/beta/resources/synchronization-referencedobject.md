---
title: Тип ресурса referencedObject
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c6e273474c70919bab3c30335a26477509eca8cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132533"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="779a7-103">Тип ресурса referencedObject</span><span class="sxs-lookup"><span data-stu-id="779a7-103">referencedObject resource type</span></span>

<span data-ttu-id="779a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="779a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="779a7-105">Описывает ссылку на другой объект, определенный в том же [определении каталога.](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="779a7-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="779a7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="779a7-106">Properties</span></span>

| <span data-ttu-id="779a7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="779a7-107">Property</span></span>                   | <span data-ttu-id="779a7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="779a7-108">Type</span></span>                      | <span data-ttu-id="779a7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="779a7-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="779a7-110">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="779a7-110">referencedObjectName</span></span>        |<span data-ttu-id="779a7-111">Строка</span><span class="sxs-lookup"><span data-stu-id="779a7-111">String</span></span>                     |<span data-ttu-id="779a7-112">Имя объекта, на который ссылается ссылка.</span><span class="sxs-lookup"><span data-stu-id="779a7-112">Name of the referenced object.</span></span> <span data-ttu-id="779a7-113">Должен соответствовать одному из объектов в [определении каталога.](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="779a7-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="779a7-114">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="779a7-114">referencedProperty</span></span>          |<span data-ttu-id="779a7-115">Строка</span><span class="sxs-lookup"><span data-stu-id="779a7-115">String</span></span>                     |<span data-ttu-id="779a7-116">**В настоящее время не поддерживается.**</span><span class="sxs-lookup"><span data-stu-id="779a7-116">**Currently not supported**.</span></span> <span data-ttu-id="779a7-117">Имя свойства в объекте, на который ссылается ссылка, значение для которого используется в качестве ссылки.</span><span class="sxs-lookup"><span data-stu-id="779a7-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="779a7-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="779a7-118">JSON representation</span></span>

<span data-ttu-id="779a7-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="779a7-119">The following is a JSON representation of the resource.</span></span>

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
            


