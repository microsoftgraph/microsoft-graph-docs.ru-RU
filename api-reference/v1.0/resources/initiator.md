---
title: Тип ресурса инициатора
description: Описывает, кто и что инициировал событие подготовка.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b1450b8344907f321b4620a909561fb5253b26b0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240775"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="22be9-103">Тип ресурса инициатора</span><span class="sxs-lookup"><span data-stu-id="22be9-103">initiator resource type</span></span>

<span data-ttu-id="22be9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22be9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22be9-105">Описывает, кто и что инициировал событие подготовка.</span><span class="sxs-lookup"><span data-stu-id="22be9-105">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="22be9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="22be9-106">Properties</span></span>

| <span data-ttu-id="22be9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="22be9-107">Property</span></span>     | <span data-ttu-id="22be9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="22be9-108">Type</span></span>        | <span data-ttu-id="22be9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="22be9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22be9-110">displayName</span><span class="sxs-lookup"><span data-stu-id="22be9-110">displayName</span></span>|<span data-ttu-id="22be9-111">Строка</span><span class="sxs-lookup"><span data-stu-id="22be9-111">String</span></span>|<span data-ttu-id="22be9-112">Имя лица или службы, которая инициировала событие подготовка.</span><span class="sxs-lookup"><span data-stu-id="22be9-112">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="22be9-113">id</span><span class="sxs-lookup"><span data-stu-id="22be9-113">id</span></span>|<span data-ttu-id="22be9-114">Строка</span><span class="sxs-lookup"><span data-stu-id="22be9-114">String</span></span>|<span data-ttu-id="22be9-115">Уникально идентифицирует человека или службу, которая инициировала событие подготовка.</span><span class="sxs-lookup"><span data-stu-id="22be9-115">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="22be9-116">initiatorType</span><span class="sxs-lookup"><span data-stu-id="22be9-116">initiatorType</span></span>|<span data-ttu-id="22be9-117">initiatorType</span><span class="sxs-lookup"><span data-stu-id="22be9-117">initiatorType</span></span>| <span data-ttu-id="22be9-118">Тип инициатора.</span><span class="sxs-lookup"><span data-stu-id="22be9-118">Type of initiator.</span></span> <span data-ttu-id="22be9-119">Возможные значения: `user`, `application`, `system`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="22be9-119">Possible values are: `user`, `application`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22be9-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="22be9-120">JSON representation</span></span>

<span data-ttu-id="22be9-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22be9-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


