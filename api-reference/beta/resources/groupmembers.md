---
title: сложный тип Граупмемберс
description: Определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 576fd13962dcafaa876225393cc9165e5ef2ece2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078439"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="0ec1a-103">сложный тип Граупмемберс</span><span class="sxs-lookup"><span data-stu-id="0ec1a-103">groupMembers complex type</span></span>

<span data-ttu-id="0ec1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ec1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ec1a-105">Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ec1a-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="0ec1a-106">`@odata.type`Значение " `#microsoft.graph.groupMembers` " указывает, что этот тип определяет коллекцию пользователей в клиенте, которые будут разрешены запрашивающими лицами, утверждающими лицами или рецензентами, которые являются участниками определенной группы.</span><span class="sxs-lookup"><span data-stu-id="0ec1a-106">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="0ec1a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ec1a-107">Properties</span></span>

| <span data-ttu-id="0ec1a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ec1a-108">Property</span></span>                     | <span data-ttu-id="0ec1a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0ec1a-109">Type</span></span>                      | <span data-ttu-id="0ec1a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0ec1a-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="0ec1a-111">id</span><span class="sxs-lookup"><span data-stu-id="0ec1a-111">id</span></span> |<span data-ttu-id="0ec1a-112">String</span><span class="sxs-lookup"><span data-stu-id="0ec1a-112">String</span></span> | <span data-ttu-id="0ec1a-113">Идентификатор группы в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0ec1a-113">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="0ec1a-114">description</span><span class="sxs-lookup"><span data-stu-id="0ec1a-114">description</span></span> |<span data-ttu-id="0ec1a-115">String</span><span class="sxs-lookup"><span data-stu-id="0ec1a-115">String</span></span> | <span data-ttu-id="0ec1a-116">Имя группы в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0ec1a-116">The name of the group in Azure AD.</span></span> <span data-ttu-id="0ec1a-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ec1a-117">Read only.</span></span> |
| <span data-ttu-id="0ec1a-118">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="0ec1a-118">isBackup</span></span> | <span data-ttu-id="0ec1a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ec1a-119">Boolean</span></span> | <span data-ttu-id="0ec1a-120">Для **граупмемберс** на этапе утверждения данное свойство указывает, что участники группы являются утверждающим резервным утверждающим.</span><span class="sxs-lookup"><span data-stu-id="0ec1a-120">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ec1a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ec1a-121">JSON representation</span></span>


<span data-ttu-id="0ec1a-122">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ec1a-122">The following is a JSON representation of the type.</span></span>

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


