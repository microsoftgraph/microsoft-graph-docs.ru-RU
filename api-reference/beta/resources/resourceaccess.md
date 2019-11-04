---
title: Тип ресурса Ресаурцеакцесс
description: Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: d0d04ba99c0132a0f305bb0fdcaa5e32071d7554
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939266"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="48a01-103">Тип ресурса Ресаурцеакцесс</span><span class="sxs-lookup"><span data-stu-id="48a01-103">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48a01-104">Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением.</span><span class="sxs-lookup"><span data-stu-id="48a01-104">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="48a01-105">Свойство **ресаурцеакцесс** типа [рекуиредресаурцеакцесс](requiredresourceaccess.md) является коллекцией **ресаурцеакцесс**.</span><span class="sxs-lookup"><span data-stu-id="48a01-105">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="48a01-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48a01-106">JSON representation</span></span>

<span data-ttu-id="48a01-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="48a01-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="48a01-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="48a01-108">Properties</span></span>
| <span data-ttu-id="48a01-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="48a01-109">Property</span></span>     | <span data-ttu-id="48a01-110">Тип</span><span class="sxs-lookup"><span data-stu-id="48a01-110">Type</span></span>   |<span data-ttu-id="48a01-111">Описание</span><span class="sxs-lookup"><span data-stu-id="48a01-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48a01-112">id</span><span class="sxs-lookup"><span data-stu-id="48a01-112">id</span></span>|<span data-ttu-id="48a01-113">GUID</span><span class="sxs-lookup"><span data-stu-id="48a01-113">Guid</span></span>|<span data-ttu-id="48a01-114">Уникальный идентификатор для одного из экземпляров [oauth2PermissionScopes](permissionscope.md) или [аппроле](approle.md) , предоставляемых приложением ресурсов.</span><span class="sxs-lookup"><span data-stu-id="48a01-114">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="48a01-115">type</span><span class="sxs-lookup"><span data-stu-id="48a01-115">type</span></span>|<span data-ttu-id="48a01-116">String</span><span class="sxs-lookup"><span data-stu-id="48a01-116">String</span></span>|<span data-ttu-id="48a01-117">Указывает, ссылается ли свойство **ID** на объект [oauth2PermissionScopes](permissionscope.md) или [аппроле](approle.md).</span><span class="sxs-lookup"><span data-stu-id="48a01-117">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="48a01-118">Возможные значения: "Scope" или "role".</span><span class="sxs-lookup"><span data-stu-id="48a01-118">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
