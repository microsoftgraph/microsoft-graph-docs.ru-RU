---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 304d5a27714d7e6e02183b372814c8cb16c4e0b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446795"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="e11b1-103">Тип ресурса userIdentity</span><span class="sxs-lookup"><span data-stu-id="e11b1-103">userIdentity resource type</span></span>

<span data-ttu-id="e11b1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e11b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e11b1-105">В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.</span><span class="sxs-lookup"><span data-stu-id="e11b1-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="e11b1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e11b1-106">Properties</span></span>

| <span data-ttu-id="e11b1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e11b1-107">Property</span></span>     | <span data-ttu-id="e11b1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e11b1-108">Type</span></span>   |<span data-ttu-id="e11b1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e11b1-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e11b1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e11b1-110">displayName</span></span> | <span data-ttu-id="e11b1-111">Строка</span><span class="sxs-lookup"><span data-stu-id="e11b1-111">String</span></span> | <span data-ttu-id="e11b1-112">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e11b1-112">The identity's display name.</span></span> <span data-ttu-id="e11b1-113">Обратите внимание, что эта возможность не всегда доступна или не актуальна.</span><span class="sxs-lookup"><span data-stu-id="e11b1-113">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="e11b1-114">id</span><span class="sxs-lookup"><span data-stu-id="e11b1-114">id</span></span>          | <span data-ttu-id="e11b1-115">String</span><span class="sxs-lookup"><span data-stu-id="e11b1-115">String</span></span> | <span data-ttu-id="e11b1-116">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e11b1-116">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="e11b1-117">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e11b1-117">ipAddress</span></span>   | <span data-ttu-id="e11b1-118">String</span><span class="sxs-lookup"><span data-stu-id="e11b1-118">String</span></span>| <span data-ttu-id="e11b1-119">IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).</span><span class="sxs-lookup"><span data-stu-id="e11b1-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="e11b1-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e11b1-120">userPrincipalName</span></span> | <span data-ttu-id="e11b1-121">String</span><span class="sxs-lookup"><span data-stu-id="e11b1-121">String</span></span>  | <span data-ttu-id="e11b1-122">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="e11b1-122">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="e11b1-123">**Примечание:** В некоторых случаях уникальный идентификатор может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="e11b1-123">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="e11b1-124">В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="e11b1-124">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e11b1-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e11b1-125">JSON representation</span></span>

<span data-ttu-id="e11b1-126">Ниже показано представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e11b1-126">Here is a JSON representation of the type.</span></span>

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
