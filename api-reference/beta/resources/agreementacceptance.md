---
title: Тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28f3c0adccb853ac8daddca9aaad70a2c0b35e2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508382"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="ca2a7-103">Тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="ca2a7-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="ca2a7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ca2a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca2a7-105">Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ca2a7-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="ca2a7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca2a7-106">Properties</span></span>
| <span data-ttu-id="ca2a7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca2a7-107">Property</span></span>     | <span data-ttu-id="ca2a7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ca2a7-108">Type</span></span>        | <span data-ttu-id="ca2a7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2a7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca2a7-110">агриментфилеид</span><span class="sxs-lookup"><span data-stu-id="ca2a7-110">agreementFileId</span></span>|<span data-ttu-id="ca2a7-111">String</span><span class="sxs-lookup"><span data-stu-id="ca2a7-111">String</span></span>|<span data-ttu-id="ca2a7-112">Идентификатор файла соглашения, принятого пользователем.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="ca2a7-113">агриментид</span><span class="sxs-lookup"><span data-stu-id="ca2a7-113">agreementId</span></span>|<span data-ttu-id="ca2a7-114">String</span><span class="sxs-lookup"><span data-stu-id="ca2a7-114">String</span></span>|<span data-ttu-id="ca2a7-115">Идентификатор соглашения.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-115">ID of the agreement.</span></span>|
|<span data-ttu-id="ca2a7-116">id</span><span class="sxs-lookup"><span data-stu-id="ca2a7-116">id</span></span>|<span data-ttu-id="ca2a7-117">String</span><span class="sxs-lookup"><span data-stu-id="ca2a7-117">String</span></span>| <span data-ttu-id="ca2a7-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-118">Read-only.</span></span>|
|<span data-ttu-id="ca2a7-119">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca2a7-119">recordedDateTime</span></span>|<span data-ttu-id="ca2a7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca2a7-120">DateTimeOffset</span></span>|<span data-ttu-id="ca2a7-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ca2a7-123">состояние</span><span class="sxs-lookup"><span data-stu-id="ca2a7-123">state</span></span>|<span data-ttu-id="ca2a7-124">строка</span><span class="sxs-lookup"><span data-stu-id="ca2a7-124">string</span></span>| <span data-ttu-id="ca2a7-125">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-125">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="ca2a7-126">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ca2a7-126">userDisplayName</span></span>|<span data-ttu-id="ca2a7-127">String</span><span class="sxs-lookup"><span data-stu-id="ca2a7-127">String</span></span>|<span data-ttu-id="ca2a7-128">Отображаемое имя пользователя, когда оно было записано.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-128">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="ca2a7-129">userEmail</span><span class="sxs-lookup"><span data-stu-id="ca2a7-129">userEmail</span></span>|<span data-ttu-id="ca2a7-130">String</span><span class="sxs-lookup"><span data-stu-id="ca2a7-130">String</span></span>|<span data-ttu-id="ca2a7-131">Сообщение электронной почты пользователя, когда сообщение о принятии было записано.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-131">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="ca2a7-132">userId</span><span class="sxs-lookup"><span data-stu-id="ca2a7-132">userId</span></span>|<span data-ttu-id="ca2a7-133">String</span><span class="sxs-lookup"><span data-stu-id="ca2a7-133">String</span></span>|<span data-ttu-id="ca2a7-134">Идентификатор пользователя, который принял соглашение.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-134">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="ca2a7-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ca2a7-135">userPrincipalName</span></span>|<span data-ttu-id="ca2a7-136">String</span><span class="sxs-lookup"><span data-stu-id="ca2a7-136">String</span></span>|<span data-ttu-id="ca2a7-137">Имя участника-пользователя, когда оно было записано.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-137">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca2a7-138">Связи</span><span class="sxs-lookup"><span data-stu-id="ca2a7-138">Relationships</span></span>
<span data-ttu-id="ca2a7-139">Нет</span><span class="sxs-lookup"><span data-stu-id="ca2a7-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ca2a7-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca2a7-140">JSON representation</span></span>

<span data-ttu-id="ca2a7-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca2a7-141">The following is a JSON representation of the resource.</span></span>

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
