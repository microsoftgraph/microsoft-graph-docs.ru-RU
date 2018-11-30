---
title: Тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в области компании настраиваемые условия использования на платформе Azure Active Directory (Azure AD).
ms.openlocfilehash: 23221fe88a65b003c8d26aca99eaf1f03d935722
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074813"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="23e9f-103">Тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="23e9f-103">agreementAcceptance resource type</span></span>

> <span data-ttu-id="23e9f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23e9f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23e9f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23e9f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23e9f-106">Представляет текущее состояние пользователя в области компании настраиваемые условия использования на платформе Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="23e9f-106">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="23e9f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="23e9f-107">Properties</span></span>
| <span data-ttu-id="23e9f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="23e9f-108">Property</span></span>     | <span data-ttu-id="23e9f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="23e9f-109">Type</span></span>        | <span data-ttu-id="23e9f-110">Description</span><span class="sxs-lookup"><span data-stu-id="23e9f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23e9f-111">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="23e9f-111">agreementFileId</span></span>|<span data-ttu-id="23e9f-112">String</span><span class="sxs-lookup"><span data-stu-id="23e9f-112">String</span></span>|<span data-ttu-id="23e9f-113">Идентификатор файла соглашения, принятия пользователем.</span><span class="sxs-lookup"><span data-stu-id="23e9f-113">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="23e9f-114">agreementId</span><span class="sxs-lookup"><span data-stu-id="23e9f-114">agreementId</span></span>|<span data-ttu-id="23e9f-115">String</span><span class="sxs-lookup"><span data-stu-id="23e9f-115">String</span></span>|<span data-ttu-id="23e9f-116">Идентификатор соглашения.</span><span class="sxs-lookup"><span data-stu-id="23e9f-116">ID of the agreement.</span></span>|
|<span data-ttu-id="23e9f-117">id</span><span class="sxs-lookup"><span data-stu-id="23e9f-117">id</span></span>|<span data-ttu-id="23e9f-118">String</span><span class="sxs-lookup"><span data-stu-id="23e9f-118">String</span></span>| <span data-ttu-id="23e9f-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23e9f-119">Read-only.</span></span>|
|<span data-ttu-id="23e9f-120">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="23e9f-120">recordedDateTime</span></span>|<span data-ttu-id="23e9f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23e9f-121">DateTimeOffset</span></span>|<span data-ttu-id="23e9f-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="23e9f-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="23e9f-124">state</span><span class="sxs-lookup"><span data-stu-id="23e9f-124">state</span></span>|<span data-ttu-id="23e9f-125">string</span><span class="sxs-lookup"><span data-stu-id="23e9f-125">string</span></span>| <span data-ttu-id="23e9f-126">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="23e9f-126">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="23e9f-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="23e9f-127">userDisplayName</span></span>|<span data-ttu-id="23e9f-128">String</span><span class="sxs-lookup"><span data-stu-id="23e9f-128">String</span></span>|<span data-ttu-id="23e9f-129">Отображаемое имя пользователя, когда было записывается.</span><span class="sxs-lookup"><span data-stu-id="23e9f-129">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="23e9f-130">userEmail</span><span class="sxs-lookup"><span data-stu-id="23e9f-130">userEmail</span></span>|<span data-ttu-id="23e9f-131">String</span><span class="sxs-lookup"><span data-stu-id="23e9f-131">String</span></span>|<span data-ttu-id="23e9f-132">Адрес электронной почты пользователя, когда было записывается.</span><span class="sxs-lookup"><span data-stu-id="23e9f-132">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="23e9f-133">userId</span><span class="sxs-lookup"><span data-stu-id="23e9f-133">userId</span></span>|<span data-ttu-id="23e9f-134">String</span><span class="sxs-lookup"><span data-stu-id="23e9f-134">String</span></span>|<span data-ttu-id="23e9f-135">Идентификатор пользователя, который принятия соглашения.</span><span class="sxs-lookup"><span data-stu-id="23e9f-135">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="23e9f-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23e9f-136">userPrincipalName</span></span>|<span data-ttu-id="23e9f-137">String</span><span class="sxs-lookup"><span data-stu-id="23e9f-137">String</span></span>|<span data-ttu-id="23e9f-138">Имя участника-пользователя, когда было записывается.</span><span class="sxs-lookup"><span data-stu-id="23e9f-138">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23e9f-139">Связи</span><span class="sxs-lookup"><span data-stu-id="23e9f-139">Relationships</span></span>
<span data-ttu-id="23e9f-140">Нет</span><span class="sxs-lookup"><span data-stu-id="23e9f-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="23e9f-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23e9f-141">JSON representation</span></span>

<span data-ttu-id="23e9f-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23e9f-142">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
