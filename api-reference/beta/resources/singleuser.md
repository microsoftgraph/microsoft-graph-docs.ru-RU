---
title: сложный тип singleUser
description: Определяет пользователя в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или рецензента.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e1982eef048e1f68f579df7f2ebc6b0975f2f0b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761046"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="4fb41-103">сложный тип singleUser</span><span class="sxs-lookup"><span data-stu-id="4fb41-103">singleUser complex type</span></span>

<span data-ttu-id="4fb41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fb41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fb41-105">Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакета [доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4fb41-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="4fb41-106">Это значение указывает на то, что этот набор пользователей определяет конкретного пользователя в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или  `@odata.type` `#microsoft.graph.singleUser` рецензента.</span><span class="sxs-lookup"><span data-stu-id="4fb41-106">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="4fb41-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fb41-107">Properties</span></span>

<span data-ttu-id="4fb41-108">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="4fb41-108">This type has the following properties:</span></span>

| <span data-ttu-id="4fb41-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fb41-109">Property</span></span>                     | <span data-ttu-id="4fb41-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4fb41-110">Type</span></span>                      | <span data-ttu-id="4fb41-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4fb41-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="4fb41-112">id</span><span class="sxs-lookup"><span data-stu-id="4fb41-112">id</span></span> |<span data-ttu-id="4fb41-113">String</span><span class="sxs-lookup"><span data-stu-id="4fb41-113">String</span></span> | <span data-ttu-id="4fb41-114">ID пользователя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4fb41-114">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="4fb41-115">description</span><span class="sxs-lookup"><span data-stu-id="4fb41-115">description</span></span> |<span data-ttu-id="4fb41-116">String</span><span class="sxs-lookup"><span data-stu-id="4fb41-116">String</span></span> | <span data-ttu-id="4fb41-117">Имя пользователя в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4fb41-117">The name of the user in Azure AD.</span></span> <span data-ttu-id="4fb41-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fb41-118">Read only.</span></span> |
| <span data-ttu-id="4fb41-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="4fb41-119">isBackup</span></span> | <span data-ttu-id="4fb41-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb41-120">Boolean</span></span> | <span data-ttu-id="4fb41-121">Для **одного пользователя на** стадии утверждения указывает, является ли пользователь резервным кодом.</span><span class="sxs-lookup"><span data-stu-id="4fb41-121">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4fb41-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fb41-122">JSON representation</span></span>

<span data-ttu-id="4fb41-123">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="4fb41-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "id": "string (identifier)",
  "description": "string"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleUser complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


