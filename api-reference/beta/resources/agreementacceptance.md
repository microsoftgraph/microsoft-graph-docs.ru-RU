---
title: тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с использованием Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 55e0be212c0f7a9e655acff03606eda851a0e5c6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722484"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="e02b1-103">тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="e02b1-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="e02b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e02b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e02b1-105">Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с использованием Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e02b1-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="e02b1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e02b1-106">Properties</span></span>
| <span data-ttu-id="e02b1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e02b1-107">Property</span></span>     | <span data-ttu-id="e02b1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e02b1-108">Type</span></span>        | <span data-ttu-id="e02b1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e02b1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e02b1-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="e02b1-110">agreementFileId</span></span>|<span data-ttu-id="e02b1-111">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-111">String</span></span>|<span data-ttu-id="e02b1-112">ID файла соглашения, принятого пользователем.</span><span class="sxs-lookup"><span data-stu-id="e02b1-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="e02b1-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="e02b1-113">agreementId</span></span>|<span data-ttu-id="e02b1-114">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-114">String</span></span>|<span data-ttu-id="e02b1-115">ID соглашения.</span><span class="sxs-lookup"><span data-stu-id="e02b1-115">ID of the agreement.</span></span>|
|<span data-ttu-id="e02b1-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e02b1-116">deviceDisplayName</span></span>|<span data-ttu-id="e02b1-117">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-117">String</span></span>|<span data-ttu-id="e02b1-118">Отображающее имя устройства, используемого для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="e02b1-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="e02b1-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="e02b1-119">deviceId</span></span>|<span data-ttu-id="e02b1-120">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-120">String</span></span>|<span data-ttu-id="e02b1-121">Уникальный идентификатор устройства, используемого для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="e02b1-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="e02b1-122">deviceOSType</span><span class="sxs-lookup"><span data-stu-id="e02b1-122">deviceOSType</span></span>|<span data-ttu-id="e02b1-123">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-123">String</span></span>|<span data-ttu-id="e02b1-124">Операционная система, используемая для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="e02b1-124">The operating system used for accepting the agreement.</span></span>|
|<span data-ttu-id="e02b1-125">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="e02b1-125">deviceOSVersion</span></span>|<span data-ttu-id="e02b1-126">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-126">String</span></span>|<span data-ttu-id="e02b1-127">Версия операционной системы устройства, используемого для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="e02b1-127">The operating system version of the device used for accepting the agreement.</span></span>    |
|<span data-ttu-id="e02b1-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e02b1-128">expirationDateTime</span></span>|<span data-ttu-id="e02b1-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e02b1-129">DateTimeOffset</span></span>|<span data-ttu-id="e02b1-130">Срок действия даты принятия.</span><span class="sxs-lookup"><span data-stu-id="e02b1-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="e02b1-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e02b1-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e02b1-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e02b1-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e02b1-133">id</span><span class="sxs-lookup"><span data-stu-id="e02b1-133">id</span></span>|<span data-ttu-id="e02b1-134">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-134">String</span></span>| <span data-ttu-id="e02b1-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e02b1-135">Read-only.</span></span>|
|<span data-ttu-id="e02b1-136">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="e02b1-136">recordedDateTime</span></span>|<span data-ttu-id="e02b1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e02b1-137">DateTimeOffset</span></span>|<span data-ttu-id="e02b1-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e02b1-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e02b1-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e02b1-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e02b1-140">состояние</span><span class="sxs-lookup"><span data-stu-id="e02b1-140">state</span></span>|<span data-ttu-id="e02b1-141">string</span><span class="sxs-lookup"><span data-stu-id="e02b1-141">string</span></span>| <span data-ttu-id="e02b1-142">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="e02b1-142">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="e02b1-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e02b1-143">userDisplayName</span></span>|<span data-ttu-id="e02b1-144">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-144">String</span></span>|<span data-ttu-id="e02b1-145">Отображение имени пользователя при записи приемки.</span><span class="sxs-lookup"><span data-stu-id="e02b1-145">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e02b1-146">userEmail</span><span class="sxs-lookup"><span data-stu-id="e02b1-146">userEmail</span></span>|<span data-ttu-id="e02b1-147">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-147">String</span></span>|<span data-ttu-id="e02b1-148">Электронная почта пользователя при записи принятия.</span><span class="sxs-lookup"><span data-stu-id="e02b1-148">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e02b1-149">userId</span><span class="sxs-lookup"><span data-stu-id="e02b1-149">userId</span></span>|<span data-ttu-id="e02b1-150">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-150">String</span></span>|<span data-ttu-id="e02b1-151">ID пользователя, который принял соглашение.</span><span class="sxs-lookup"><span data-stu-id="e02b1-151">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="e02b1-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e02b1-152">userPrincipalName</span></span>|<span data-ttu-id="e02b1-153">String</span><span class="sxs-lookup"><span data-stu-id="e02b1-153">String</span></span>|<span data-ttu-id="e02b1-154">UPN пользователя при записи принятия.</span><span class="sxs-lookup"><span data-stu-id="e02b1-154">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e02b1-155">Связи</span><span class="sxs-lookup"><span data-stu-id="e02b1-155">Relationships</span></span>
<span data-ttu-id="e02b1-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e02b1-156">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e02b1-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e02b1-157">JSON representation</span></span>

<span data-ttu-id="e02b1-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e02b1-158">The following is a JSON representation of the resource.</span></span>

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


