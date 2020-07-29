---
title: Тип ресурса Домаинидентитисаурце
description: Тип Домаинидентитисаурце определяет домен, не относящийся к клиенту, в качестве источника удостоверения для подключенной Организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 134f0ae3c382c879b48d468545dd40f2d6bd101b
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510380"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="b5755-103">Тип ресурса Домаинидентитисаурце</span><span class="sxs-lookup"><span data-stu-id="b5755-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="b5755-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5755-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5755-105">Используется в источниках удостоверений [коннектедорганизатион](connectedOrganization.md).</span><span class="sxs-lookup"><span data-stu-id="b5755-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="b5755-106">`@odata.type`Значение `#microsoft.graph.domainIdentitySource` указывает на то, что этот тип определяет домен как источник идентификаторов для подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="b5755-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="b5755-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5755-107">Properties</span></span>

| <span data-ttu-id="b5755-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5755-108">Property</span></span>                     | <span data-ttu-id="b5755-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b5755-109">Type</span></span>                      | <span data-ttu-id="b5755-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b5755-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="b5755-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b5755-111">displayName</span></span> |<span data-ttu-id="b5755-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b5755-112">String</span></span> | <span data-ttu-id="b5755-113">Имя источника удостоверений, как правило, также доменное имя.</span><span class="sxs-lookup"><span data-stu-id="b5755-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="b5755-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5755-114">Read only.</span></span> |
| <span data-ttu-id="b5755-115">domainName</span><span class="sxs-lookup"><span data-stu-id="b5755-115">domainName</span></span> |<span data-ttu-id="b5755-116">String</span><span class="sxs-lookup"><span data-stu-id="b5755-116">String</span></span> | <span data-ttu-id="b5755-117">Доменное имя.</span><span class="sxs-lookup"><span data-stu-id="b5755-117">The domain name.</span></span> <span data-ttu-id="b5755-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5755-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b5755-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b5755-119">Relationships</span></span>

<span data-ttu-id="b5755-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b5755-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5755-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b5755-121">JSON representation</span></span>

<span data-ttu-id="b5755-122">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5755-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
