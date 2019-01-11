---
title: Тип ресурса referencedObject
description: Описывает ссылку на другой объект, определенных в одно и то же определение каталога.
localization_priority: Normal
ms.openlocfilehash: 5a2aa2dcc358c856c18ea2ce9871ec634194ce54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821037"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="ca0c7-103">Тип ресурса referencedObject</span><span class="sxs-lookup"><span data-stu-id="ca0c7-103">referencedObject resource type</span></span>

> <span data-ttu-id="ca0c7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca0c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca0c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca0c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca0c7-106">Описывает ссылку на другой объект, определенных в одно и то же [Определение каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ca0c7-106">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ca0c7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca0c7-107">Properties</span></span>

| <span data-ttu-id="ca0c7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca0c7-108">Property</span></span>                   | <span data-ttu-id="ca0c7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ca0c7-109">Type</span></span>                      | <span data-ttu-id="ca0c7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ca0c7-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="ca0c7-111">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="ca0c7-111">referencedObjectName</span></span>        |<span data-ttu-id="ca0c7-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ca0c7-112">String</span></span>                     |<span data-ttu-id="ca0c7-113">Имя объекта, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="ca0c7-113">Name of the referenced object.</span></span> <span data-ttu-id="ca0c7-114">Должно соответствовать одному из объектов в [каталоге определения](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ca0c7-114">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="ca0c7-115">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="ca0c7-115">referencedProperty</span></span>          |<span data-ttu-id="ca0c7-116">Строка</span><span class="sxs-lookup"><span data-stu-id="ca0c7-116">String</span></span>                     |<span data-ttu-id="ca0c7-117">**В настоящее время не поддерживается**.</span><span class="sxs-lookup"><span data-stu-id="ca0c7-117">**Currently not supported**.</span></span> <span data-ttu-id="ca0c7-118">Имя свойства в этом объекте, значение которой используется в качестве ссылки.</span><span class="sxs-lookup"><span data-stu-id="ca0c7-118">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca0c7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca0c7-119">JSON representation</span></span>

<span data-ttu-id="ca0c7-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca0c7-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            
