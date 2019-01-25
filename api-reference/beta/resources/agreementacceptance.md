---
title: Тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в области компании настраиваемые условия использования на платформе Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: 884a6b7dcf4dcc8f00aa927dd9d486c074b64183
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518872"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="b1f31-103">Тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="b1f31-103">agreementAcceptance resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1f31-104">Представляет текущее состояние пользователя в области компании настраиваемые условия использования на платформе Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b1f31-104">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="b1f31-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1f31-105">Properties</span></span>
| <span data-ttu-id="b1f31-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1f31-106">Property</span></span>     | <span data-ttu-id="b1f31-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b1f31-107">Type</span></span>        | <span data-ttu-id="b1f31-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b1f31-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1f31-109">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="b1f31-109">agreementFileId</span></span>|<span data-ttu-id="b1f31-110">String</span><span class="sxs-lookup"><span data-stu-id="b1f31-110">String</span></span>|<span data-ttu-id="b1f31-111">Идентификатор файла соглашения, принятия пользователем.</span><span class="sxs-lookup"><span data-stu-id="b1f31-111">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="b1f31-112">agreementId</span><span class="sxs-lookup"><span data-stu-id="b1f31-112">agreementId</span></span>|<span data-ttu-id="b1f31-113">String</span><span class="sxs-lookup"><span data-stu-id="b1f31-113">String</span></span>|<span data-ttu-id="b1f31-114">Идентификатор соглашения.</span><span class="sxs-lookup"><span data-stu-id="b1f31-114">ID of the agreement.</span></span>|
|<span data-ttu-id="b1f31-115">id</span><span class="sxs-lookup"><span data-stu-id="b1f31-115">id</span></span>|<span data-ttu-id="b1f31-116">Строка</span><span class="sxs-lookup"><span data-stu-id="b1f31-116">String</span></span>| <span data-ttu-id="b1f31-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1f31-117">Read-only.</span></span>|
|<span data-ttu-id="b1f31-118">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1f31-118">recordedDateTime</span></span>|<span data-ttu-id="b1f31-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1f31-119">DateTimeOffset</span></span>|<span data-ttu-id="b1f31-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b1f31-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1f31-122">state</span><span class="sxs-lookup"><span data-stu-id="b1f31-122">state</span></span>|<span data-ttu-id="b1f31-123">string</span><span class="sxs-lookup"><span data-stu-id="b1f31-123">string</span></span>| <span data-ttu-id="b1f31-124">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="b1f31-124">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="b1f31-125">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1f31-125">userDisplayName</span></span>|<span data-ttu-id="b1f31-126">String</span><span class="sxs-lookup"><span data-stu-id="b1f31-126">String</span></span>|<span data-ttu-id="b1f31-127">Отображаемое имя пользователя, когда было записывается.</span><span class="sxs-lookup"><span data-stu-id="b1f31-127">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="b1f31-128">userEmail</span><span class="sxs-lookup"><span data-stu-id="b1f31-128">userEmail</span></span>|<span data-ttu-id="b1f31-129">String</span><span class="sxs-lookup"><span data-stu-id="b1f31-129">String</span></span>|<span data-ttu-id="b1f31-130">Адрес электронной почты пользователя, когда было записывается.</span><span class="sxs-lookup"><span data-stu-id="b1f31-130">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="b1f31-131">userId</span><span class="sxs-lookup"><span data-stu-id="b1f31-131">userId</span></span>|<span data-ttu-id="b1f31-132">String</span><span class="sxs-lookup"><span data-stu-id="b1f31-132">String</span></span>|<span data-ttu-id="b1f31-133">Идентификатор пользователя, который принятия соглашения.</span><span class="sxs-lookup"><span data-stu-id="b1f31-133">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="b1f31-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1f31-134">userPrincipalName</span></span>|<span data-ttu-id="b1f31-135">String</span><span class="sxs-lookup"><span data-stu-id="b1f31-135">String</span></span>|<span data-ttu-id="b1f31-136">Имя участника-пользователя, когда было записывается.</span><span class="sxs-lookup"><span data-stu-id="b1f31-136">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1f31-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="b1f31-137">Relationships</span></span>
<span data-ttu-id="b1f31-138">Нет</span><span class="sxs-lookup"><span data-stu-id="b1f31-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1f31-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1f31-139">JSON representation</span></span>

<span data-ttu-id="b1f31-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1f31-140">The following is a JSON representation of the resource.</span></span>

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
