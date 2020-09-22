---
title: Тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: f3bad64c1cb691c5a5f5c1c5377bcb4e0188f184
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067510"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="e95e6-103">Тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="e95e6-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="e95e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e95e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e95e6-105">Представляет текущее состояние пользователя в пределах области настраиваемых терминов компании на платформе Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e95e6-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="e95e6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e95e6-106">Properties</span></span>
| <span data-ttu-id="e95e6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e95e6-107">Property</span></span>     | <span data-ttu-id="e95e6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e95e6-108">Type</span></span>        | <span data-ttu-id="e95e6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e95e6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e95e6-110">агриментфилеид</span><span class="sxs-lookup"><span data-stu-id="e95e6-110">agreementFileId</span></span>|<span data-ttu-id="e95e6-111">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-111">String</span></span>|<span data-ttu-id="e95e6-112">Идентификатор файла соглашения, принятого пользователем.</span><span class="sxs-lookup"><span data-stu-id="e95e6-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="e95e6-113">агриментид</span><span class="sxs-lookup"><span data-stu-id="e95e6-113">agreementId</span></span>|<span data-ttu-id="e95e6-114">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-114">String</span></span>|<span data-ttu-id="e95e6-115">Идентификатор соглашения.</span><span class="sxs-lookup"><span data-stu-id="e95e6-115">ID of the agreement.</span></span>|
|<span data-ttu-id="e95e6-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e95e6-116">deviceDisplayName</span></span>|<span data-ttu-id="e95e6-117">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-117">String</span></span>|<span data-ttu-id="e95e6-118">Отображаемое имя устройства, используемое для принятия соглашения.</span><span class="sxs-lookup"><span data-stu-id="e95e6-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="e95e6-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="e95e6-119">deviceId</span></span>|<span data-ttu-id="e95e6-120">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-120">String</span></span>|<span data-ttu-id="e95e6-121">Уникальный идентификатор устройства, используемого для принятия соглашения.</span><span class="sxs-lookup"><span data-stu-id="e95e6-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="e95e6-122">девицеостипе</span><span class="sxs-lookup"><span data-stu-id="e95e6-122">deviceOSType</span></span>|<span data-ttu-id="e95e6-123">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-123">String</span></span>|<span data-ttu-id="e95e6-124">Операционная система, используемая для принятия соглашения.</span><span class="sxs-lookup"><span data-stu-id="e95e6-124">The operating system used for accepting the agreement.</span></span>|
|<span data-ttu-id="e95e6-125">девицеосверсион</span><span class="sxs-lookup"><span data-stu-id="e95e6-125">deviceOSVersion</span></span>|<span data-ttu-id="e95e6-126">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-126">String</span></span>|<span data-ttu-id="e95e6-127">Версия операционной системы устройства, используемая для принятия соглашения.</span><span class="sxs-lookup"><span data-stu-id="e95e6-127">The operating system version of the device used for accepting the agreement.</span></span>    |
|<span data-ttu-id="e95e6-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e95e6-128">expirationDateTime</span></span>|<span data-ttu-id="e95e6-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e95e6-129">DateTimeOffset</span></span>|<span data-ttu-id="e95e6-130">Дата и время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="e95e6-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="e95e6-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e95e6-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e95e6-132">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e95e6-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e95e6-133">id</span><span class="sxs-lookup"><span data-stu-id="e95e6-133">id</span></span>|<span data-ttu-id="e95e6-134">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-134">String</span></span>| <span data-ttu-id="e95e6-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e95e6-135">Read-only.</span></span>|
|<span data-ttu-id="e95e6-136">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="e95e6-136">recordedDateTime</span></span>|<span data-ttu-id="e95e6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e95e6-137">DateTimeOffset</span></span>|<span data-ttu-id="e95e6-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e95e6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e95e6-140">состояние</span><span class="sxs-lookup"><span data-stu-id="e95e6-140">state</span></span>|<span data-ttu-id="e95e6-141">string</span><span class="sxs-lookup"><span data-stu-id="e95e6-141">string</span></span>| <span data-ttu-id="e95e6-142">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="e95e6-142">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="e95e6-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e95e6-143">userDisplayName</span></span>|<span data-ttu-id="e95e6-144">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-144">String</span></span>|<span data-ttu-id="e95e6-145">Отображаемое имя пользователя, когда оно было записано.</span><span class="sxs-lookup"><span data-stu-id="e95e6-145">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e95e6-146">userEmail</span><span class="sxs-lookup"><span data-stu-id="e95e6-146">userEmail</span></span>|<span data-ttu-id="e95e6-147">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-147">String</span></span>|<span data-ttu-id="e95e6-148">Сообщение электронной почты пользователя, когда сообщение о принятии было записано.</span><span class="sxs-lookup"><span data-stu-id="e95e6-148">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e95e6-149">userId</span><span class="sxs-lookup"><span data-stu-id="e95e6-149">userId</span></span>|<span data-ttu-id="e95e6-150">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-150">String</span></span>|<span data-ttu-id="e95e6-151">Идентификатор пользователя, который принял соглашение.</span><span class="sxs-lookup"><span data-stu-id="e95e6-151">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="e95e6-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e95e6-152">userPrincipalName</span></span>|<span data-ttu-id="e95e6-153">String</span><span class="sxs-lookup"><span data-stu-id="e95e6-153">String</span></span>|<span data-ttu-id="e95e6-154">Имя участника-пользователя, когда оно было записано.</span><span class="sxs-lookup"><span data-stu-id="e95e6-154">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e95e6-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="e95e6-155">Relationships</span></span>
<span data-ttu-id="e95e6-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e95e6-156">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e95e6-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e95e6-157">JSON representation</span></span>

<span data-ttu-id="e95e6-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e95e6-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
      "id": "String (identifier)",
      "agreementId": "String",
      "userId": "String",
      "deviceId": "String",
      "deviceDisplayName": "String",
      "deviceOSType": "String",
      "deviceOSVersion": "String",
      "agreementFileId": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userEmail": "String",
      "recordedDateTime": "String (timestamp)",
      "expirationDateTime": "String",
      "state": "String"
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


