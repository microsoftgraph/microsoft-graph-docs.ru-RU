---
title: connectedOrganizationMembers сложный тип
description: Тип connectedOrganizationMembers определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивателя, утверждения или рецензента.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 725926bc39583bda653294f0cc917ea7d2f08a45
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761820"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="35242-103">connectedOrganizationMembers сложный тип</span><span class="sxs-lookup"><span data-stu-id="35242-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="35242-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35242-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35242-105">Используется в параметрах запросов политики назначения [пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35242-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="35242-106">Значение указывает, что этот тип определяет коллекцию пользователей, связанных с подключенной организацией, которым будет разрешено `@odata.type` `#microsoft.graph.connectedOrganizationMembers` запрашивать пакет доступа. [](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="35242-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a [connected organization](connectedorganization.md), who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="35242-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="35242-107">Properties</span></span>

<span data-ttu-id="35242-108">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="35242-108">This type has the following properties:</span></span>

| <span data-ttu-id="35242-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="35242-109">Property</span></span>                     | <span data-ttu-id="35242-110">Тип</span><span class="sxs-lookup"><span data-stu-id="35242-110">Type</span></span>                      | <span data-ttu-id="35242-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35242-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="35242-112">id</span><span class="sxs-lookup"><span data-stu-id="35242-112">id</span></span> |<span data-ttu-id="35242-113">String</span><span class="sxs-lookup"><span data-stu-id="35242-113">String</span></span> | <span data-ttu-id="35242-114">ID связанной организации в управлении правами.</span><span class="sxs-lookup"><span data-stu-id="35242-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="35242-115">description</span><span class="sxs-lookup"><span data-stu-id="35242-115">description</span></span> |<span data-ttu-id="35242-116">String</span><span class="sxs-lookup"><span data-stu-id="35242-116">String</span></span> | <span data-ttu-id="35242-117">Имя связанной организации.</span><span class="sxs-lookup"><span data-stu-id="35242-117">The name of the connected organization.</span></span> <span data-ttu-id="35242-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35242-118">Read only.</span></span> |
| <span data-ttu-id="35242-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="35242-119">isBackup</span></span> | <span data-ttu-id="35242-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="35242-120">Boolean</span></span> | <span data-ttu-id="35242-121">Не используется в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="35242-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35242-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35242-122">JSON representation</span></span>

<span data-ttu-id="35242-123">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="35242-123">The following is a JSON representation of the type.</span></span>

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


