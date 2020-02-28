---
title: сложный тип Граупмемберс
description: Определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ca1b7b0a2ae4021dc2def637e0326044ab8749e
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331424"
---
# <a name="groupmembers-complex-type"></a><span data-ttu-id="f20f6-103">сложный тип Граупмемберс</span><span class="sxs-lookup"><span data-stu-id="f20f6-103">groupMembers complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f20f6-104">Используется в параметрах просмотра запроса, утверждения и назначения для [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f20f6-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="f20f6-105">`@odata.type` Значение "`#microsoft.graph.groupMembers`" указывает, что этот тип определяет коллекцию пользователей в клиенте, которые будут разрешены запрашивающими лицами, утверждающими лицами или рецензентами, которые являются участниками определенной группы.</span><span class="sxs-lookup"><span data-stu-id="f20f6-105">The `@odata.type` value "`#microsoft.graph.groupMembers`" indicates that this type identifies a collection of users in the tenant who will be allowed as requestor, approver, or reviewer, who are the members of a specific group.</span></span>

## <a name="properties"></a><span data-ttu-id="f20f6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f20f6-106">Properties</span></span>

| <span data-ttu-id="f20f6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f20f6-107">Property</span></span>                     | <span data-ttu-id="f20f6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f20f6-108">Type</span></span>                      | <span data-ttu-id="f20f6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f20f6-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="f20f6-110">id</span><span class="sxs-lookup"><span data-stu-id="f20f6-110">id</span></span> |<span data-ttu-id="f20f6-111">Строка</span><span class="sxs-lookup"><span data-stu-id="f20f6-111">String</span></span> | <span data-ttu-id="f20f6-112">Идентификатор группы в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f20f6-112">The ID of the group in Azure AD.</span></span> |
| <span data-ttu-id="f20f6-113">description</span><span class="sxs-lookup"><span data-stu-id="f20f6-113">description</span></span> |<span data-ttu-id="f20f6-114">String</span><span class="sxs-lookup"><span data-stu-id="f20f6-114">String</span></span> | <span data-ttu-id="f20f6-115">Имя группы в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f20f6-115">The name of the group in Azure AD.</span></span> <span data-ttu-id="f20f6-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f20f6-116">Read only.</span></span> |
| <span data-ttu-id="f20f6-117">Создание резервной копии</span><span class="sxs-lookup"><span data-stu-id="f20f6-117">isBackup</span></span> | <span data-ttu-id="f20f6-118">Логический</span><span class="sxs-lookup"><span data-stu-id="f20f6-118">Boolean</span></span> | <span data-ttu-id="f20f6-119">Для **граупмемберс** на этапе утверждения данное свойство указывает, что участники группы являются утверждающим резервным утверждающим.</span><span class="sxs-lookup"><span data-stu-id="f20f6-119">For **groupMembers** in an approval stage, this property indicates that the group members are a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f20f6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f20f6-120">JSON representation</span></span>


<span data-ttu-id="f20f6-121">Ниже представлено представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f20f6-121">The following is a JSON representation of the type.</span></span>

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
