---
title: Тип ресурса Принтусеридентити
description: Представляет удостоверение пользователя в универсальной службе печати. Сопоставление с пользователем Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8a695bed829d6c7e8825898da366737427195e1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070662"
---
# <a name="printuseridentity-resource-type"></a><span data-ttu-id="1cb20-104">Тип ресурса Принтусеридентити</span><span class="sxs-lookup"><span data-stu-id="1cb20-104">printUserIdentity resource type</span></span>

<span data-ttu-id="1cb20-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cb20-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cb20-106">Представляет удостоверение пользователя в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="1cb20-106">Represents a user identity within the Universal Print service.</span></span> <span data-ttu-id="1cb20-107">Сопоставляется с [пользователем Azure Active Directory (Azure AD)](user.md).</span><span class="sxs-lookup"><span data-stu-id="1cb20-107">Maps to an [Azure Active Directory (Azure AD) user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1cb20-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cb20-108">Properties</span></span>
| <span data-ttu-id="1cb20-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cb20-109">Property</span></span>     | <span data-ttu-id="1cb20-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1cb20-110">Type</span></span>        | <span data-ttu-id="1cb20-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb20-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1cb20-112">id</span><span class="sxs-lookup"><span data-stu-id="1cb20-112">id</span></span>|<span data-ttu-id="1cb20-113">String</span><span class="sxs-lookup"><span data-stu-id="1cb20-113">String</span></span>|<span data-ttu-id="1cb20-114">Идентификатор Принтусеридентити.</span><span class="sxs-lookup"><span data-stu-id="1cb20-114">The printUserIdentity's identifier.</span></span> <span data-ttu-id="1cb20-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cb20-115">Read-only.</span></span>|
|<span data-ttu-id="1cb20-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1cb20-116">displayName</span></span>|<span data-ttu-id="1cb20-117">String</span><span class="sxs-lookup"><span data-stu-id="1cb20-117">String</span></span>|<span data-ttu-id="1cb20-118">Отображаемое имя Принтусеридентити.</span><span class="sxs-lookup"><span data-stu-id="1cb20-118">The printUserIdentity's display name.</span></span>|
|<span data-ttu-id="1cb20-119">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1cb20-119">ipAddress</span></span>|<span data-ttu-id="1cb20-120">String</span><span class="sxs-lookup"><span data-stu-id="1cb20-120">String</span></span>|<span data-ttu-id="1cb20-121">IP-адрес Принтусеридентити.</span><span class="sxs-lookup"><span data-stu-id="1cb20-121">The printUserIdentity' IP address.</span></span> <span data-ttu-id="1cb20-122">Не заполнено.</span><span class="sxs-lookup"><span data-stu-id="1cb20-122">Not populated.</span></span>|
|<span data-ttu-id="1cb20-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1cb20-123">userPrincipalName</span></span>|<span data-ttu-id="1cb20-124">String</span><span class="sxs-lookup"><span data-stu-id="1cb20-124">String</span></span>|<span data-ttu-id="1cb20-125">Имя участника-пользователя Принтусеридентити (UPN).</span><span class="sxs-lookup"><span data-stu-id="1cb20-125">The printUserIdentity's user principal name (UPN).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cb20-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1cb20-126">JSON representation</span></span>

<span data-ttu-id="1cb20-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cb20-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUserIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUserIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


