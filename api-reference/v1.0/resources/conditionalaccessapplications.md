---
title: тип ресурса conditionalAccessApplications
description: Представляет приложения и действия пользователей, включенные и исключенные из области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3d864acfdd794bc5bcb914c460b29800c4a86291
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962506"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="d6149-103">тип ресурса conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="d6149-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="d6149-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6149-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6149-105">Представляет приложения и действия пользователей, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="d6149-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="d6149-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6149-106">Properties</span></span>

| <span data-ttu-id="d6149-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6149-107">Property</span></span>     | <span data-ttu-id="d6149-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d6149-108">Type</span></span>        | <span data-ttu-id="d6149-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d6149-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d6149-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="d6149-110">includeApplications</span></span> | <span data-ttu-id="d6149-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6149-111">String collection</span></span> | <span data-ttu-id="d6149-112">Список ID приложений, к который применяется политика, если явно не исключено (в исключенииApplications).</span><span class="sxs-lookup"><span data-stu-id="d6149-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="d6149-113">Также можно установить `All` .</span><span class="sxs-lookup"><span data-stu-id="d6149-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="d6149-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="d6149-114">excludeApplications</span></span> | <span data-ttu-id="d6149-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6149-115">String collection</span></span> | <span data-ttu-id="d6149-116">Список ID приложений явно исключен из политики.</span><span class="sxs-lookup"><span data-stu-id="d6149-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="d6149-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="d6149-117">includeUserActions</span></span> | <span data-ttu-id="d6149-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6149-118">String collection</span></span> | <span data-ttu-id="d6149-119">Действия пользователя, которые необходимо включить.</span><span class="sxs-lookup"><span data-stu-id="d6149-119">User actions to include.</span></span> <span data-ttu-id="d6149-120">Поддерживаемые значения `urn:user:registersecurityinfo` и `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="d6149-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |

## <a name="relationships"></a><span data-ttu-id="d6149-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d6149-121">Relationships</span></span>

<span data-ttu-id="d6149-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d6149-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6149-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d6149-123">JSON representation</span></span>

<span data-ttu-id="d6149-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6149-124">The following is a JSON representation of the resource.</span></span>

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

