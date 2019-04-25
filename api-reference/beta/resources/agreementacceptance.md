---
title: Тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: 884a6b7dcf4dcc8f00aa927dd9d486c074b64183
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544066"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="e6624-103">Тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="e6624-103">agreementAcceptance resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6624-104">Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e6624-104">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="e6624-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6624-105">Properties</span></span>
| <span data-ttu-id="e6624-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6624-106">Property</span></span>     | <span data-ttu-id="e6624-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e6624-107">Type</span></span>        | <span data-ttu-id="e6624-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e6624-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6624-109">Агриментфилеид</span><span class="sxs-lookup"><span data-stu-id="e6624-109">agreementFileId</span></span>|<span data-ttu-id="e6624-110">String</span><span class="sxs-lookup"><span data-stu-id="e6624-110">String</span></span>|<span data-ttu-id="e6624-111">Идентификатор файла соглашения, принятого пользователем.</span><span class="sxs-lookup"><span data-stu-id="e6624-111">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="e6624-112">Агриментид</span><span class="sxs-lookup"><span data-stu-id="e6624-112">agreementId</span></span>|<span data-ttu-id="e6624-113">String</span><span class="sxs-lookup"><span data-stu-id="e6624-113">String</span></span>|<span data-ttu-id="e6624-114">Идентификатор соглашения.</span><span class="sxs-lookup"><span data-stu-id="e6624-114">ID of the agreement.</span></span>|
|<span data-ttu-id="e6624-115">id</span><span class="sxs-lookup"><span data-stu-id="e6624-115">id</span></span>|<span data-ttu-id="e6624-116">String</span><span class="sxs-lookup"><span data-stu-id="e6624-116">String</span></span>| <span data-ttu-id="e6624-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6624-117">Read-only.</span></span>|
|<span data-ttu-id="e6624-118">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6624-118">recordedDateTime</span></span>|<span data-ttu-id="e6624-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6624-119">DateTimeOffset</span></span>|<span data-ttu-id="e6624-p101">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e6624-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e6624-122">состояние</span><span class="sxs-lookup"><span data-stu-id="e6624-122">state</span></span>|<span data-ttu-id="e6624-123">string</span><span class="sxs-lookup"><span data-stu-id="e6624-123">string</span></span>| <span data-ttu-id="e6624-124">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="e6624-124">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="e6624-125">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6624-125">userDisplayName</span></span>|<span data-ttu-id="e6624-126">String</span><span class="sxs-lookup"><span data-stu-id="e6624-126">String</span></span>|<span data-ttu-id="e6624-127">Отображаемое имя пользователя, когда оно было записано.</span><span class="sxs-lookup"><span data-stu-id="e6624-127">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e6624-128">userEmail</span><span class="sxs-lookup"><span data-stu-id="e6624-128">userEmail</span></span>|<span data-ttu-id="e6624-129">String</span><span class="sxs-lookup"><span data-stu-id="e6624-129">String</span></span>|<span data-ttu-id="e6624-130">Сообщение электронной почты пользователя, когда сообщение о принятии было записано.</span><span class="sxs-lookup"><span data-stu-id="e6624-130">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e6624-131">userId</span><span class="sxs-lookup"><span data-stu-id="e6624-131">userId</span></span>|<span data-ttu-id="e6624-132">String</span><span class="sxs-lookup"><span data-stu-id="e6624-132">String</span></span>|<span data-ttu-id="e6624-133">Идентификатор пользователя, который принял соглашение.</span><span class="sxs-lookup"><span data-stu-id="e6624-133">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="e6624-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6624-134">userPrincipalName</span></span>|<span data-ttu-id="e6624-135">String</span><span class="sxs-lookup"><span data-stu-id="e6624-135">String</span></span>|<span data-ttu-id="e6624-136">ИМЯ участника-пользователя, когда оно было записано.</span><span class="sxs-lookup"><span data-stu-id="e6624-136">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6624-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="e6624-137">Relationships</span></span>
<span data-ttu-id="e6624-138">Нет</span><span class="sxs-lookup"><span data-stu-id="e6624-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6624-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e6624-139">JSON representation</span></span>

<span data-ttu-id="e6624-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6624-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
  "agreementFileId": "String",
  "agreementId": "String",
  "id": "String (identifier)",
  "recordedDateTime": "String (timestamp)",
  "state": "string",
  "userDisplayName": "String",
  "userEmail": "String",
  "userId": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementacceptance.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
