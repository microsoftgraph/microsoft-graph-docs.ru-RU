---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e72f5338f7281188b7023aed342dd34ee57595e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033504"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="0dc73-103">Тип ресурса userIdentity</span><span class="sxs-lookup"><span data-stu-id="0dc73-103">userIdentity resource type</span></span>

<span data-ttu-id="0dc73-104">В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.</span><span class="sxs-lookup"><span data-stu-id="0dc73-104">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="0dc73-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0dc73-105">Properties</span></span>

| <span data-ttu-id="0dc73-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0dc73-106">Property</span></span>     | <span data-ttu-id="0dc73-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0dc73-107">Type</span></span>   |<span data-ttu-id="0dc73-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0dc73-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0dc73-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0dc73-109">displayName</span></span> | <span data-ttu-id="0dc73-110">Строка</span><span class="sxs-lookup"><span data-stu-id="0dc73-110">String</span></span> | <span data-ttu-id="0dc73-111">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0dc73-111">The identity's display name.</span></span> <span data-ttu-id="0dc73-112">Обратите внимание, что эта возможность не всегда доступна или не актуальна.</span><span class="sxs-lookup"><span data-stu-id="0dc73-112">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="0dc73-113">id</span><span class="sxs-lookup"><span data-stu-id="0dc73-113">id</span></span>          | <span data-ttu-id="0dc73-114">String</span><span class="sxs-lookup"><span data-stu-id="0dc73-114">String</span></span> | <span data-ttu-id="0dc73-115">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0dc73-115">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="0dc73-116">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0dc73-116">ipAddress</span></span>   | <span data-ttu-id="0dc73-117">String</span><span class="sxs-lookup"><span data-stu-id="0dc73-117">String</span></span>| <span data-ttu-id="0dc73-118">IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).</span><span class="sxs-lookup"><span data-stu-id="0dc73-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="0dc73-119">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0dc73-119">userPrincipalName</span></span> | <span data-ttu-id="0dc73-120">String</span><span class="sxs-lookup"><span data-stu-id="0dc73-120">String</span></span>  | <span data-ttu-id="0dc73-121">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="0dc73-121">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="0dc73-122">**Примечание:** В некоторых случаях уникальный идентификатор может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="0dc73-122">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="0dc73-123">В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="0dc73-123">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dc73-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0dc73-124">JSON representation</span></span>

<span data-ttu-id="0dc73-125">Ниже показано представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0dc73-125">Here is a JSON representation of the type.</span></span>

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
