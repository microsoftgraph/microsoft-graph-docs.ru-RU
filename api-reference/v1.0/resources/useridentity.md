---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 32bfb6d7a92ce566d10809277f19f82e45ffc1a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015388"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="6aca3-103">Тип ресурса userIdentity</span><span class="sxs-lookup"><span data-stu-id="6aca3-103">userIdentity resource type</span></span>

<span data-ttu-id="6aca3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aca3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6aca3-105">В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.</span><span class="sxs-lookup"><span data-stu-id="6aca3-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="6aca3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6aca3-106">Properties</span></span>

| <span data-ttu-id="6aca3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6aca3-107">Property</span></span>     | <span data-ttu-id="6aca3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6aca3-108">Type</span></span>   |<span data-ttu-id="6aca3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6aca3-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6aca3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6aca3-110">displayName</span></span> | <span data-ttu-id="6aca3-111">String</span><span class="sxs-lookup"><span data-stu-id="6aca3-111">String</span></span> | <span data-ttu-id="6aca3-112">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="6aca3-112">The identity's display name.</span></span> <span data-ttu-id="6aca3-113">Обратите внимание, что эта возможность не всегда доступна или не актуальна.</span><span class="sxs-lookup"><span data-stu-id="6aca3-113">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="6aca3-114">id</span><span class="sxs-lookup"><span data-stu-id="6aca3-114">id</span></span>          | <span data-ttu-id="6aca3-115">String</span><span class="sxs-lookup"><span data-stu-id="6aca3-115">String</span></span> | <span data-ttu-id="6aca3-116">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="6aca3-116">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="6aca3-117">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6aca3-117">ipAddress</span></span>   | <span data-ttu-id="6aca3-118">String</span><span class="sxs-lookup"><span data-stu-id="6aca3-118">String</span></span>| <span data-ttu-id="6aca3-119">IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).</span><span class="sxs-lookup"><span data-stu-id="6aca3-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="6aca3-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6aca3-120">userPrincipalName</span></span> | <span data-ttu-id="6aca3-121">String</span><span class="sxs-lookup"><span data-stu-id="6aca3-121">String</span></span>  | <span data-ttu-id="6aca3-122">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="6aca3-122">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="6aca3-123">**Примечание:** В некоторых случаях уникальный идентификатор может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="6aca3-123">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="6aca3-124">В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="6aca3-124">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6aca3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6aca3-125">JSON representation</span></span>

<span data-ttu-id="6aca3-126">Ниже показано представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aca3-126">Here is a JSON representation of the type.</span></span>

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
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

