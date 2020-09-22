---
title: сложный тип Коннектедорганизатионмемберс
description: Тип Коннектедорганизатионмемберс определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d2df6b91ebcbc65f03ee39103768bdfad04df62f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027197"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="fcea4-103">сложный тип Коннектедорганизатионмемберс</span><span class="sxs-lookup"><span data-stu-id="fcea4-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="fcea4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcea4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcea4-105">Используется в параметрах запроса [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fcea4-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="fcea4-106">`@odata.type`Значение `#microsoft.graph.connectedOrganizationMembers` указывает на то, что этот тип определяет коллекцию пользователей, которые связаны с [подключенной организацией](connectedorganization.md)и могут запрашивать пакет Access.</span><span class="sxs-lookup"><span data-stu-id="fcea4-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a [connected organization](connectedorganization.md), who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="fcea4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcea4-107">Properties</span></span>

<span data-ttu-id="fcea4-108">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="fcea4-108">This type has the following properties:</span></span>

| <span data-ttu-id="fcea4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcea4-109">Property</span></span>                     | <span data-ttu-id="fcea4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fcea4-110">Type</span></span>                      | <span data-ttu-id="fcea4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fcea4-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="fcea4-112">id</span><span class="sxs-lookup"><span data-stu-id="fcea4-112">id</span></span> |<span data-ttu-id="fcea4-113">String</span><span class="sxs-lookup"><span data-stu-id="fcea4-113">String</span></span> | <span data-ttu-id="fcea4-114">Идентификатор подключенной Организации в управлении обслуживанием.</span><span class="sxs-lookup"><span data-stu-id="fcea4-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="fcea4-115">description</span><span class="sxs-lookup"><span data-stu-id="fcea4-115">description</span></span> |<span data-ttu-id="fcea4-116">String</span><span class="sxs-lookup"><span data-stu-id="fcea4-116">String</span></span> | <span data-ttu-id="fcea4-117">Имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="fcea4-117">The name of the connected organization.</span></span> <span data-ttu-id="fcea4-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcea4-118">Read only.</span></span> |
| <span data-ttu-id="fcea4-119">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="fcea4-119">isBackup</span></span> | <span data-ttu-id="fcea4-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="fcea4-120">Boolean</span></span> | <span data-ttu-id="fcea4-121">Не используется в данный момент.</span><span class="sxs-lookup"><span data-stu-id="fcea4-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fcea4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcea4-122">JSON representation</span></span>

<span data-ttu-id="fcea4-123">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcea4-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
  "isBackup": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


