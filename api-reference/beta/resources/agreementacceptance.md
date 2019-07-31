---
title: Тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 58ed332429d7976b75929b433d57bd77536b9e70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013453"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="8d0c8-103">Тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="8d0c8-103">agreementAcceptance resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d0c8-104">Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8d0c8-104">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="8d0c8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d0c8-105">Properties</span></span>
| <span data-ttu-id="8d0c8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d0c8-106">Property</span></span>     | <span data-ttu-id="8d0c8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8d0c8-107">Type</span></span>        | <span data-ttu-id="8d0c8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8d0c8-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d0c8-109">Агриментфилеид</span><span class="sxs-lookup"><span data-stu-id="8d0c8-109">agreementFileId</span></span>|<span data-ttu-id="8d0c8-110">String</span><span class="sxs-lookup"><span data-stu-id="8d0c8-110">String</span></span>|<span data-ttu-id="8d0c8-111">Идентификатор файла соглашения, принятого пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-111">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="8d0c8-112">Агриментид</span><span class="sxs-lookup"><span data-stu-id="8d0c8-112">agreementId</span></span>|<span data-ttu-id="8d0c8-113">String</span><span class="sxs-lookup"><span data-stu-id="8d0c8-113">String</span></span>|<span data-ttu-id="8d0c8-114">Идентификатор соглашения.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-114">ID of the agreement.</span></span>|
|<span data-ttu-id="8d0c8-115">id</span><span class="sxs-lookup"><span data-stu-id="8d0c8-115">id</span></span>|<span data-ttu-id="8d0c8-116">String</span><span class="sxs-lookup"><span data-stu-id="8d0c8-116">String</span></span>| <span data-ttu-id="8d0c8-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-117">Read-only.</span></span>|
|<span data-ttu-id="8d0c8-118">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d0c8-118">recordedDateTime</span></span>|<span data-ttu-id="8d0c8-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d0c8-119">DateTimeOffset</span></span>|<span data-ttu-id="8d0c8-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8d0c8-122">состояние</span><span class="sxs-lookup"><span data-stu-id="8d0c8-122">state</span></span>|<span data-ttu-id="8d0c8-123">string</span><span class="sxs-lookup"><span data-stu-id="8d0c8-123">string</span></span>| <span data-ttu-id="8d0c8-124">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-124">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="8d0c8-125">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8d0c8-125">userDisplayName</span></span>|<span data-ttu-id="8d0c8-126">String</span><span class="sxs-lookup"><span data-stu-id="8d0c8-126">String</span></span>|<span data-ttu-id="8d0c8-127">Отображаемое имя пользователя, когда оно было записано.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-127">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="8d0c8-128">userEmail</span><span class="sxs-lookup"><span data-stu-id="8d0c8-128">userEmail</span></span>|<span data-ttu-id="8d0c8-129">String</span><span class="sxs-lookup"><span data-stu-id="8d0c8-129">String</span></span>|<span data-ttu-id="8d0c8-130">Сообщение электронной почты пользователя, когда сообщение о принятии было записано.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-130">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="8d0c8-131">userId</span><span class="sxs-lookup"><span data-stu-id="8d0c8-131">userId</span></span>|<span data-ttu-id="8d0c8-132">String</span><span class="sxs-lookup"><span data-stu-id="8d0c8-132">String</span></span>|<span data-ttu-id="8d0c8-133">Идентификатор пользователя, который принял соглашение.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-133">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="8d0c8-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8d0c8-134">userPrincipalName</span></span>|<span data-ttu-id="8d0c8-135">String</span><span class="sxs-lookup"><span data-stu-id="8d0c8-135">String</span></span>|<span data-ttu-id="8d0c8-136">Имя участника-пользователя, когда оно было записано.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-136">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d0c8-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="8d0c8-137">Relationships</span></span>
<span data-ttu-id="8d0c8-138">Нет</span><span class="sxs-lookup"><span data-stu-id="8d0c8-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8d0c8-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d0c8-139">JSON representation</span></span>

<span data-ttu-id="8d0c8-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d0c8-140">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
