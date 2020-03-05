---
title: Тип ресурса Референцедобжект
description: Описывает ссылку на другой объект, определенный в том же определении каталога.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c27830b1ee9762b52a7f24a0785e1b19010181d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520123"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="489e4-103">Тип ресурса Референцедобжект</span><span class="sxs-lookup"><span data-stu-id="489e4-103">referencedObject resource type</span></span>

<span data-ttu-id="489e4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="489e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="489e4-105">Описывает ссылку на другой объект, определенный в том же [определении каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="489e4-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="489e4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="489e4-106">Properties</span></span>

| <span data-ttu-id="489e4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="489e4-107">Property</span></span>                   | <span data-ttu-id="489e4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="489e4-108">Type</span></span>                      | <span data-ttu-id="489e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="489e4-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="489e4-110">референцедобжектнаме</span><span class="sxs-lookup"><span data-stu-id="489e4-110">referencedObjectName</span></span>        |<span data-ttu-id="489e4-111">String</span><span class="sxs-lookup"><span data-stu-id="489e4-111">String</span></span>                     |<span data-ttu-id="489e4-112">Имя объекта, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="489e4-112">Name of the referenced object.</span></span> <span data-ttu-id="489e4-113">Должен сопоставлять один из объектов в [определении каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="489e4-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="489e4-114">референцедпроперти</span><span class="sxs-lookup"><span data-stu-id="489e4-114">referencedProperty</span></span>          |<span data-ttu-id="489e4-115">String</span><span class="sxs-lookup"><span data-stu-id="489e4-115">String</span></span>                     |<span data-ttu-id="489e4-116">**В настоящее время не поддерживается**.</span><span class="sxs-lookup"><span data-stu-id="489e4-116">**Currently not supported**.</span></span> <span data-ttu-id="489e4-117">Имя свойства в объекте, на который указывает ссылка, значение, которое используется в качестве ссылки.</span><span class="sxs-lookup"><span data-stu-id="489e4-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="489e4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="489e4-118">JSON representation</span></span>

<span data-ttu-id="489e4-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="489e4-119">The following is a JSON representation of the resource.</span></span>

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
            
