---
title: Тип ресурса conditionalAccessApplications
description: Представляет приложения и действия пользователей, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 42ceafb6c786666378d1327ecd158a04559d7f0d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132162"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="4caf4-103">Тип ресурса conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="4caf4-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="4caf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4caf4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4caf4-105">Представляет приложения и действия пользователей, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="4caf4-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="4caf4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4caf4-106">Properties</span></span>

| <span data-ttu-id="4caf4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4caf4-107">Property</span></span>     | <span data-ttu-id="4caf4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4caf4-108">Type</span></span>        | <span data-ttu-id="4caf4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4caf4-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4caf4-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="4caf4-110">includeApplications</span></span> | <span data-ttu-id="4caf4-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4caf4-111">String collection</span></span> | <span data-ttu-id="4caf4-112">Список ИД приложений, к которых применяется политика, за исключением явно исключенных (в excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="4caf4-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="4caf4-113">Также может быть установлено в `All` .</span><span class="sxs-lookup"><span data-stu-id="4caf4-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="4caf4-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="4caf4-114">excludeApplications</span></span> | <span data-ttu-id="4caf4-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4caf4-115">String collection</span></span> | <span data-ttu-id="4caf4-116">Список явно исключенных из политики ИД приложений.</span><span class="sxs-lookup"><span data-stu-id="4caf4-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="4caf4-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="4caf4-117">includeUserActions</span></span> | <span data-ttu-id="4caf4-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4caf4-118">String collection</span></span> | <span data-ttu-id="4caf4-119">Действия пользователей, которые необходимо включить.</span><span class="sxs-lookup"><span data-stu-id="4caf4-119">User actions to include.</span></span> <span data-ttu-id="4caf4-120">Пример: `urn:user:registersecurityinfo`</span><span class="sxs-lookup"><span data-stu-id="4caf4-120">For example, `urn:user:registersecurityinfo`</span></span> |

## <a name="relationships"></a><span data-ttu-id="4caf4-121">Связи</span><span class="sxs-lookup"><span data-stu-id="4caf4-121">Relationships</span></span>

<span data-ttu-id="4caf4-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4caf4-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4caf4-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4caf4-123">JSON representation</span></span>

<span data-ttu-id="4caf4-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4caf4-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

