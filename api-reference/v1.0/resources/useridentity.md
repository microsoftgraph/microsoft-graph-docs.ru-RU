---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD это сведения о пользователях, которые инициировали или были затронуты действиями аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 814b7106bf738711099d6d6e8d5e821b7b638318
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292163"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="d2981-103">Тип ресурса userIdentity</span><span class="sxs-lookup"><span data-stu-id="d2981-103">userIdentity resource type</span></span>

<span data-ttu-id="d2981-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2981-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2981-105">В контексте журнала аудита Azure AD это сведения о пользователях, которые инициировали или были затронуты действиями аудита.</span><span class="sxs-lookup"><span data-stu-id="d2981-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="d2981-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2981-106">Properties</span></span>

| <span data-ttu-id="d2981-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2981-107">Property</span></span>     | <span data-ttu-id="d2981-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d2981-108">Type</span></span>   |<span data-ttu-id="d2981-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d2981-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d2981-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d2981-110">displayName</span></span> | <span data-ttu-id="d2981-111">String</span><span class="sxs-lookup"><span data-stu-id="d2981-111">String</span></span> | <span data-ttu-id="d2981-112">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d2981-112">The identity's display name.</span></span> <span data-ttu-id="d2981-113">Обратите внимание, что это может быть не всегда доступно или не всегда в курсе.</span><span class="sxs-lookup"><span data-stu-id="d2981-113">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="d2981-114">id</span><span class="sxs-lookup"><span data-stu-id="d2981-114">id</span></span>          | <span data-ttu-id="d2981-115">String</span><span class="sxs-lookup"><span data-stu-id="d2981-115">String</span></span> | <span data-ttu-id="d2981-116">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d2981-116">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="d2981-117">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d2981-117">ipAddress</span></span>   | <span data-ttu-id="d2981-118">String</span><span class="sxs-lookup"><span data-stu-id="d2981-118">String</span></span>| <span data-ttu-id="d2981-119">Указывает IP-адрес клиента, используемый пользователем, выполнив действие (только в журнале аудита).</span><span class="sxs-lookup"><span data-stu-id="d2981-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="d2981-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d2981-120">userPrincipalName</span></span> | <span data-ttu-id="d2981-121">String</span><span class="sxs-lookup"><span data-stu-id="d2981-121">String</span></span>  | <span data-ttu-id="d2981-122">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2981-122">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="d2981-123">**Примечание.** В некоторых случаях уникальный идентификатор может быть не доступен.</span><span class="sxs-lookup"><span data-stu-id="d2981-123">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="d2981-124">В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="d2981-124">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2981-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2981-125">JSON representation</span></span>

<span data-ttu-id="d2981-126">Вот представление типа в JSON.</span><span class="sxs-lookup"><span data-stu-id="d2981-126">Here is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "ipAddress": "string",
  "userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

