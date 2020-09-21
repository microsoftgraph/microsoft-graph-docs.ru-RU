---
title: Тип ресурса Ресаурцеакцесс
description: Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: c5fb2478fbce4aeece78e70983ee15fda46ac602
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967235"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="eebab-103">Тип ресурса Ресаурцеакцесс</span><span class="sxs-lookup"><span data-stu-id="eebab-103">resourceAccess resource type</span></span>

<span data-ttu-id="eebab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eebab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eebab-105">Указывает область разрешений OAuth 2,0 или роль приложения, требуемую приложением.</span><span class="sxs-lookup"><span data-stu-id="eebab-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="eebab-106">Свойство **ресаурцеакцесс** типа [рекуиредресаурцеакцесс](requiredresourceaccess.md) является коллекцией **ресаурцеакцесс**.</span><span class="sxs-lookup"><span data-stu-id="eebab-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>

## <a name="properties"></a><span data-ttu-id="eebab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eebab-107">Properties</span></span>
| <span data-ttu-id="eebab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eebab-108">Property</span></span>     | <span data-ttu-id="eebab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eebab-109">Type</span></span>   |<span data-ttu-id="eebab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eebab-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eebab-111">id</span><span class="sxs-lookup"><span data-stu-id="eebab-111">id</span></span>|<span data-ttu-id="eebab-112">GUID</span><span class="sxs-lookup"><span data-stu-id="eebab-112">Guid</span></span>|<span data-ttu-id="eebab-113">Уникальный идентификатор для одного из экземпляров [oauth2PermissionScopes](permissionscope.md) или [аппроле](approle.md) , предоставляемых приложением ресурсов.</span><span class="sxs-lookup"><span data-stu-id="eebab-113">The unique identifier for one of the [oauth2PermissionScopes](permissionscope.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="eebab-114">type</span><span class="sxs-lookup"><span data-stu-id="eebab-114">type</span></span>|<span data-ttu-id="eebab-115">String</span><span class="sxs-lookup"><span data-stu-id="eebab-115">String</span></span>|<span data-ttu-id="eebab-116">Указывает, ссылается ли свойство **ID** на объект [oauth2PermissionScopes](permissionscope.md) или [аппроле](approle.md).</span><span class="sxs-lookup"><span data-stu-id="eebab-116">Specifies whether the **id** property references an [oauth2PermissionScopes](permissionscope.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="eebab-117">Возможные значения: `Scope` или `Role` .</span><span class="sxs-lookup"><span data-stu-id="eebab-117">Possible values are `Scope` or `Role`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eebab-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eebab-118">JSON representation</span></span>

<span data-ttu-id="eebab-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eebab-119">The following is a JSON representation of the resource.</span></span>

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

