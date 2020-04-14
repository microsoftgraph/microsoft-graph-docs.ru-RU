---
title: Тип ресурса Ресаурцеакцесс
description: Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: e8972ec33fdb9a509267909876bf2aaab26e8205
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453098"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="16f67-103">Тип ресурса Ресаурцеакцесс</span><span class="sxs-lookup"><span data-stu-id="16f67-103">resourceAccess resource type</span></span>

<span data-ttu-id="16f67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16f67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16f67-105">Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением.</span><span class="sxs-lookup"><span data-stu-id="16f67-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="16f67-106">Свойство **ресаурцеакцесс** типа [рекуиредресаурцеакцесс](requiredresourceaccess.md) является коллекцией **ресаурцеакцесс**.</span><span class="sxs-lookup"><span data-stu-id="16f67-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="16f67-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16f67-107">JSON representation</span></span>

<span data-ttu-id="16f67-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="16f67-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="16f67-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="16f67-109">Properties</span></span>
| <span data-ttu-id="16f67-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="16f67-110">Property</span></span>     | <span data-ttu-id="16f67-111">Тип</span><span class="sxs-lookup"><span data-stu-id="16f67-111">Type</span></span>   |<span data-ttu-id="16f67-112">Описание</span><span class="sxs-lookup"><span data-stu-id="16f67-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16f67-113">id</span><span class="sxs-lookup"><span data-stu-id="16f67-113">id</span></span>|<span data-ttu-id="16f67-114">GUID</span><span class="sxs-lookup"><span data-stu-id="16f67-114">Guid</span></span>|<span data-ttu-id="16f67-115">Уникальный идентификатор для одного из экземпляров [oauth2PermissionScopes](permissionscope.md) или [аппроле](approle.md) , предоставляемых приложением ресурсов.</span><span class="sxs-lookup"><span data-stu-id="16f67-115">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="16f67-116">type</span><span class="sxs-lookup"><span data-stu-id="16f67-116">type</span></span>|<span data-ttu-id="16f67-117">String</span><span class="sxs-lookup"><span data-stu-id="16f67-117">String</span></span>|<span data-ttu-id="16f67-118">Указывает, ссылается ли свойство **ID** на объект [oauth2PermissionScopes](permissionscope.md) или [аппроле](approle.md).</span><span class="sxs-lookup"><span data-stu-id="16f67-118">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="16f67-119">Возможные значения: "Scope" или "role".</span><span class="sxs-lookup"><span data-stu-id="16f67-119">Possible values are "scope" or "role".</span></span>|

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
