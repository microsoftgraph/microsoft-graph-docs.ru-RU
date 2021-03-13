---
title: тип ресурса ResourceAccess
description: Указывает область разрешений OAuth 2.0 или роль приложения, которая требуется приложению.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 0072bf231fe8dba66b34188952804083593afaa1
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761074"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="aeecb-103">тип ресурса ResourceAccess</span><span class="sxs-lookup"><span data-stu-id="aeecb-103">resourceAccess resource type</span></span>

<span data-ttu-id="aeecb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeecb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aeecb-105">Указывает область разрешений OAuth 2.0 или роль приложения, которая требуется приложению.</span><span class="sxs-lookup"><span data-stu-id="aeecb-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="aeecb-106">Свойство **resourceAccess** типа [requiredResourceAccess](requiredresourceaccess.md) — это коллекция **ResourceAccess.**</span><span class="sxs-lookup"><span data-stu-id="aeecb-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>

## <a name="properties"></a><span data-ttu-id="aeecb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aeecb-107">Properties</span></span>
| <span data-ttu-id="aeecb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aeecb-108">Property</span></span>     | <span data-ttu-id="aeecb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aeecb-109">Type</span></span>   |<span data-ttu-id="aeecb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aeecb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aeecb-111">id</span><span class="sxs-lookup"><span data-stu-id="aeecb-111">id</span></span>|<span data-ttu-id="aeecb-112">GUID</span><span class="sxs-lookup"><span data-stu-id="aeecb-112">Guid</span></span>|<span data-ttu-id="aeecb-113">Уникальный идентификатор для одного из [экземпляров oauth2PermissionScopes](permissionscope.md) или экземпляров [appRole,](approle.md) которые предоставляет приложение ресурса.</span><span class="sxs-lookup"><span data-stu-id="aeecb-113">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="aeecb-114">type</span><span class="sxs-lookup"><span data-stu-id="aeecb-114">type</span></span>|<span data-ttu-id="aeecb-115">String</span><span class="sxs-lookup"><span data-stu-id="aeecb-115">String</span></span>|<span data-ttu-id="aeecb-116">Указывает, ссылается ли свойство **id** на [oauth2PermissionScopes](permissionscope.md) или [appRole.](approle.md)</span><span class="sxs-lookup"><span data-stu-id="aeecb-116">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="aeecb-117">Возможные значения: `Scope` или `Role`.</span><span class="sxs-lookup"><span data-stu-id="aeecb-117">Possible values are `Scope` or `Role`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aeecb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aeecb-118">JSON representation</span></span>

<span data-ttu-id="aeecb-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aeecb-119">The following is a JSON representation of the resource.</span></span>

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


