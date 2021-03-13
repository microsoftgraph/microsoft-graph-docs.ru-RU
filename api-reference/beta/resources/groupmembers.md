---
title: сложный тип groupMembers
description: Определяет коллекцию пользователей в клиенте, которым будет разрешено в качестве запрашивателя, утверждения или рецензента.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0069cd6a8fd738c17a9035b519c4f141c3a5fa55
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761418"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="9920b-103">сложный тип groupMembers</span><span class="sxs-lookup"><span data-stu-id="9920b-103">groupMembers complex type</span></span>

<span data-ttu-id="9920b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9920b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9920b-105">Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакета [доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9920b-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="9920b-106">Значение "" указывает, что этот тип определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивателя, утверждения или рецензента, которые являются членами `@odata.type` `#microsoft.graph.groupMembers` определенной группы.</span><span class="sxs-lookup"><span data-stu-id="9920b-106">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="9920b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9920b-107">Properties</span></span>

| <span data-ttu-id="9920b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9920b-108">Property</span></span>                     | <span data-ttu-id="9920b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9920b-109">Type</span></span>                      | <span data-ttu-id="9920b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9920b-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="9920b-111">id</span><span class="sxs-lookup"><span data-stu-id="9920b-111">id</span></span> |<span data-ttu-id="9920b-112">String</span><span class="sxs-lookup"><span data-stu-id="9920b-112">String</span></span> | <span data-ttu-id="9920b-113">ID группы в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9920b-113">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="9920b-114">description</span><span class="sxs-lookup"><span data-stu-id="9920b-114">description</span></span> |<span data-ttu-id="9920b-115">String</span><span class="sxs-lookup"><span data-stu-id="9920b-115">String</span></span> | <span data-ttu-id="9920b-116">Имя группы в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9920b-116">The name of the group in Azure AD.</span></span> <span data-ttu-id="9920b-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9920b-117">Read only.</span></span> |
| <span data-ttu-id="9920b-118">isBackup</span><span class="sxs-lookup"><span data-stu-id="9920b-118">isBackup</span></span> | <span data-ttu-id="9920b-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9920b-119">Boolean</span></span> | <span data-ttu-id="9920b-120">Для **groupMembers** на стадии утверждения это свойство указывает, что участники группы являются резервным утверждением резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="9920b-120">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9920b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9920b-121">JSON representation</span></span>


<span data-ttu-id="9920b-122">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="9920b-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupMembers",
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
  "description": "groupMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


