---
title: Тип ресурса passwordCredential
description: Содержит учетные данные пароль, связанный с приложением или участника службы. Свойство **passwordCredentials** servicePrincipal сущности и сущности приложения — это коллекция **passwordCredential**.
localization_priority: Normal
ms.openlocfilehash: 900bfb8a5828d636dfa1f1abfd0348ceb4aee143
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523150"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="edc1c-104">Тип ресурса passwordCredential</span><span class="sxs-lookup"><span data-stu-id="edc1c-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edc1c-105">Содержит учетные данные пароль, связанный с приложением или участника службы.</span><span class="sxs-lookup"><span data-stu-id="edc1c-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="edc1c-106">Свойство **passwordCredentials** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **passwordCredential**.</span><span class="sxs-lookup"><span data-stu-id="edc1c-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="edc1c-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edc1c-107">JSON representation</span></span>

<span data-ttu-id="edc1c-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="edc1c-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="edc1c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="edc1c-109">Properties</span></span>
| <span data-ttu-id="edc1c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="edc1c-110">Property</span></span>     | <span data-ttu-id="edc1c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="edc1c-111">Type</span></span>   |<span data-ttu-id="edc1c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="edc1c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edc1c-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="edc1c-113">customKeyIdentifier</span></span>|<span data-ttu-id="edc1c-114">Binary</span><span class="sxs-lookup"><span data-stu-id="edc1c-114">Binary</span></span>|            |
|<span data-ttu-id="edc1c-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="edc1c-115">endDateTime</span></span>|<span data-ttu-id="edc1c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edc1c-116">DateTimeOffset</span></span>|<span data-ttu-id="edc1c-117">Дата и время истечения срока действия пароля. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="edc1c-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="edc1c-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="edc1c-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="edc1c-119">Идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="edc1c-119">keyId</span></span>|<span data-ttu-id="edc1c-120">Guid</span><span class="sxs-lookup"><span data-stu-id="edc1c-120">Guid</span></span>|            |
|<span data-ttu-id="edc1c-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="edc1c-121">startDateTime</span></span>|<span data-ttu-id="edc1c-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edc1c-122">DateTimeOffset</span></span>|<span data-ttu-id="edc1c-123">Дата и время, в которой становится допустимый пароль. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="edc1c-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="edc1c-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="edc1c-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="edc1c-125">secretText</span><span class="sxs-lookup"><span data-stu-id="edc1c-125">secretText</span></span>|<span data-ttu-id="edc1c-126">String</span><span class="sxs-lookup"><span data-stu-id="edc1c-126">String</span></span>| <span data-ttu-id="edc1c-127">Пароли должны быть 16-64 символов</span><span class="sxs-lookup"><span data-stu-id="edc1c-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="edc1c-128">подсказка</span><span class="sxs-lookup"><span data-stu-id="edc1c-128">hint</span></span>|<span data-ttu-id="edc1c-129">String</span><span class="sxs-lookup"><span data-stu-id="edc1c-129">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordcredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
