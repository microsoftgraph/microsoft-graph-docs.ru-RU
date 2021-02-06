---
title: Тип ресурса conditionalAccessApplications
description: Представляет приложения и действия пользователей, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0a787a1c22209b502e4eed68790629e2e6e1b03b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137403"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="e3695-103">Тип ресурса conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="e3695-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="e3695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3695-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3695-105">Представляет приложения и действия пользователей, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="e3695-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e3695-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3695-106">Properties</span></span>

| <span data-ttu-id="e3695-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3695-107">Property</span></span> | <span data-ttu-id="e3695-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e3695-108">Type</span></span> | <span data-ttu-id="e3695-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e3695-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e3695-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="e3695-110">includeApplications</span></span> | <span data-ttu-id="e3695-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e3695-111">String collection</span></span> | <span data-ttu-id="e3695-112">Список ИД приложений, к которых применяется политика, за исключением явно исключенных (в excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="e3695-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="e3695-113">Также может быть установлено в `All` .</span><span class="sxs-lookup"><span data-stu-id="e3695-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="e3695-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="e3695-114">excludeApplications</span></span> | <span data-ttu-id="e3695-115">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e3695-115">String collection</span></span> | <span data-ttu-id="e3695-116">Список ИД приложений, явно исключенных из политики.</span><span class="sxs-lookup"><span data-stu-id="e3695-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="e3695-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="e3695-117">includeUserActions</span></span> | <span data-ttu-id="e3695-118">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e3695-118">String collection</span></span> | <span data-ttu-id="e3695-119">Действия пользователей, которые необходимо включить.</span><span class="sxs-lookup"><span data-stu-id="e3695-119">User actions to include.</span></span> <span data-ttu-id="e3695-120">Поддерживаемые `urn:user:registersecurityinfo` значения: `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="e3695-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |

## <a name="relationships"></a><span data-ttu-id="e3695-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e3695-121">Relationships</span></span>

<span data-ttu-id="e3695-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e3695-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3695-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3695-123">JSON representation</span></span>

<span data-ttu-id="e3695-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3695-124">The following is a JSON representation of the resource.</span></span>

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

