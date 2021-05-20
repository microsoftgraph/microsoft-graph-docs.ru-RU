---
title: тип ресурса conditionalAccessApplications
description: Представляет приложения и действия пользователей, включенные и исключенные из области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d688b529e32390c2330cf8cb3558994c3e752a25
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547685"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="62bef-103">тип ресурса conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="62bef-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="62bef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62bef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62bef-105">Представляет приложения и действия пользователей, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="62bef-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="62bef-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="62bef-106">Properties</span></span>

| <span data-ttu-id="62bef-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="62bef-107">Property</span></span> | <span data-ttu-id="62bef-108">Тип</span><span class="sxs-lookup"><span data-stu-id="62bef-108">Type</span></span> | <span data-ttu-id="62bef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62bef-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="62bef-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="62bef-110">includeApplications</span></span> | <span data-ttu-id="62bef-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="62bef-111">String collection</span></span> | <span data-ttu-id="62bef-112">Список ID приложений, к который применяется политика, если явно не исключено (в исключенииApplications).</span><span class="sxs-lookup"><span data-stu-id="62bef-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="62bef-113">Также можно установить `All` .</span><span class="sxs-lookup"><span data-stu-id="62bef-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="62bef-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="62bef-114">excludeApplications</span></span> | <span data-ttu-id="62bef-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="62bef-115">String collection</span></span> | <span data-ttu-id="62bef-116">Список ID приложений явно исключен из политики.</span><span class="sxs-lookup"><span data-stu-id="62bef-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="62bef-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="62bef-117">includeUserActions</span></span> | <span data-ttu-id="62bef-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="62bef-118">String collection</span></span> | <span data-ttu-id="62bef-119">Действия пользователя, которые необходимо включить.</span><span class="sxs-lookup"><span data-stu-id="62bef-119">User actions to include.</span></span> <span data-ttu-id="62bef-120">Поддерживаемые значения `urn:user:registersecurityinfo` и `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="62bef-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |
| <span data-ttu-id="62bef-121">includeAuthenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="62bef-121">includeAuthenticationContextClassReferences</span></span> | <span data-ttu-id="62bef-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="62bef-122">String collection</span></span> | <span data-ttu-id="62bef-123">Ссылки на класс контекста проверки подлинности включаются.</span><span class="sxs-lookup"><span data-stu-id="62bef-123">Authentication context class references include.</span></span> <span data-ttu-id="62bef-124">Поддерживаемые значения `c1` проходят `c25` .</span><span class="sxs-lookup"><span data-stu-id="62bef-124">Supported values are `c1` through `c25`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="62bef-125">Связи</span><span class="sxs-lookup"><span data-stu-id="62bef-125">Relationships</span></span>

<span data-ttu-id="62bef-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="62bef-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62bef-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="62bef-127">JSON representation</span></span>

<span data-ttu-id="62bef-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62bef-128">The following is a JSON representation of the resource.</span></span>

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

