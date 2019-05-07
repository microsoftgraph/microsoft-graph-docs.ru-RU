---
title: Тип ресурса userIdentity
description: В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 018bc8ca3713822295d0acef66e8ec075d276cfe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629231"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="65a03-103">Тип ресурса userIdentity</span><span class="sxs-lookup"><span data-stu-id="65a03-103">userIdentity resource type</span></span>

<span data-ttu-id="65a03-104">В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.</span><span class="sxs-lookup"><span data-stu-id="65a03-104">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="65a03-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="65a03-105">Properties</span></span>

| <span data-ttu-id="65a03-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="65a03-106">Property</span></span>     | <span data-ttu-id="65a03-107">Тип</span><span class="sxs-lookup"><span data-stu-id="65a03-107">Type</span></span>   |<span data-ttu-id="65a03-108">Описание</span><span class="sxs-lookup"><span data-stu-id="65a03-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="65a03-109">displayName</span><span class="sxs-lookup"><span data-stu-id="65a03-109">displayName</span></span> | <span data-ttu-id="65a03-110">Строка</span><span class="sxs-lookup"><span data-stu-id="65a03-110">String</span></span> | <span data-ttu-id="65a03-111">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="65a03-111">The identity's display name.</span></span> <span data-ttu-id="65a03-112">Обратите внимание, что эта возможность не всегда доступна или не актуальна.</span><span class="sxs-lookup"><span data-stu-id="65a03-112">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="65a03-113">id</span><span class="sxs-lookup"><span data-stu-id="65a03-113">id</span></span>          | <span data-ttu-id="65a03-114">String</span><span class="sxs-lookup"><span data-stu-id="65a03-114">String</span></span> | <span data-ttu-id="65a03-115">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="65a03-115">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="65a03-116">ipAddress</span><span class="sxs-lookup"><span data-stu-id="65a03-116">ipAddress</span></span>   | <span data-ttu-id="65a03-117">String</span><span class="sxs-lookup"><span data-stu-id="65a03-117">String</span></span>| <span data-ttu-id="65a03-118">IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).</span><span class="sxs-lookup"><span data-stu-id="65a03-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="65a03-119">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65a03-119">userPrincipalName</span></span> | <span data-ttu-id="65a03-120">String</span><span class="sxs-lookup"><span data-stu-id="65a03-120">String</span></span>  | <span data-ttu-id="65a03-121">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="65a03-121">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="65a03-122">**Примечание:** В некоторых случаях уникальный идентификатор может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="65a03-122">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="65a03-123">В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="65a03-123">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65a03-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="65a03-124">JSON representation</span></span>

<span data-ttu-id="65a03-125">Ниже показано представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65a03-125">Here is a JSON representation of the type.</span></span>

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
