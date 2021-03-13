---
title: тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с использованием Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 4e00ae32078bd004ad4063a0f73ebb94b6a77f9c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761102"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="f9b54-103">тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="f9b54-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="f9b54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9b54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9b54-105">Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с использованием Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f9b54-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="f9b54-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9b54-106">Properties</span></span>
| <span data-ttu-id="f9b54-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9b54-107">Property</span></span>     | <span data-ttu-id="f9b54-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f9b54-108">Type</span></span>        | <span data-ttu-id="f9b54-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f9b54-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f9b54-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="f9b54-110">agreementFileId</span></span>|<span data-ttu-id="f9b54-111">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-111">String</span></span>|<span data-ttu-id="f9b54-112">ID файла соглашения, принятого пользователем.</span><span class="sxs-lookup"><span data-stu-id="f9b54-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="f9b54-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="f9b54-113">agreementId</span></span>|<span data-ttu-id="f9b54-114">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-114">String</span></span>|<span data-ttu-id="f9b54-115">ID соглашения.</span><span class="sxs-lookup"><span data-stu-id="f9b54-115">ID of the agreement.</span></span>|
|<span data-ttu-id="f9b54-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9b54-116">deviceDisplayName</span></span>|<span data-ttu-id="f9b54-117">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-117">String</span></span>|<span data-ttu-id="f9b54-118">Отображающее имя устройства, используемого для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="f9b54-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="f9b54-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="f9b54-119">deviceId</span></span>|<span data-ttu-id="f9b54-120">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-120">String</span></span>|<span data-ttu-id="f9b54-121">Уникальный идентификатор устройства, используемого для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="f9b54-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="f9b54-122">deviceOSType</span><span class="sxs-lookup"><span data-stu-id="f9b54-122">deviceOSType</span></span>|<span data-ttu-id="f9b54-123">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-123">String</span></span>|<span data-ttu-id="f9b54-124">Операционная система, используемая для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="f9b54-124">The operating system used for accepting the agreement.</span></span>|
|<span data-ttu-id="f9b54-125">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="f9b54-125">deviceOSVersion</span></span>|<span data-ttu-id="f9b54-126">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-126">String</span></span>|<span data-ttu-id="f9b54-127">Версия операционной системы устройства, используемого для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="f9b54-127">The operating system version of the device used for accepting the agreement.</span></span>    |
|<span data-ttu-id="f9b54-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9b54-128">expirationDateTime</span></span>|<span data-ttu-id="f9b54-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9b54-129">DateTimeOffset</span></span>|<span data-ttu-id="f9b54-130">Срок действия даты принятия.</span><span class="sxs-lookup"><span data-stu-id="f9b54-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="f9b54-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f9b54-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f9b54-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f9b54-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f9b54-133">id</span><span class="sxs-lookup"><span data-stu-id="f9b54-133">id</span></span>|<span data-ttu-id="f9b54-134">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-134">String</span></span>| <span data-ttu-id="f9b54-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9b54-135">Read-only.</span></span>|
|<span data-ttu-id="f9b54-136">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9b54-136">recordedDateTime</span></span>|<span data-ttu-id="f9b54-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9b54-137">DateTimeOffset</span></span>|<span data-ttu-id="f9b54-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f9b54-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f9b54-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f9b54-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f9b54-140">состояние</span><span class="sxs-lookup"><span data-stu-id="f9b54-140">state</span></span>|<span data-ttu-id="f9b54-141">string</span><span class="sxs-lookup"><span data-stu-id="f9b54-141">string</span></span>| <span data-ttu-id="f9b54-142">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="f9b54-142">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="f9b54-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9b54-143">userDisplayName</span></span>|<span data-ttu-id="f9b54-144">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-144">String</span></span>|<span data-ttu-id="f9b54-145">Отображение имени пользователя при записи приемки.</span><span class="sxs-lookup"><span data-stu-id="f9b54-145">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="f9b54-146">userEmail</span><span class="sxs-lookup"><span data-stu-id="f9b54-146">userEmail</span></span>|<span data-ttu-id="f9b54-147">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-147">String</span></span>|<span data-ttu-id="f9b54-148">Электронная почта пользователя при записи принятия.</span><span class="sxs-lookup"><span data-stu-id="f9b54-148">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="f9b54-149">userId</span><span class="sxs-lookup"><span data-stu-id="f9b54-149">userId</span></span>|<span data-ttu-id="f9b54-150">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-150">String</span></span>|<span data-ttu-id="f9b54-151">ID пользователя, который принял соглашение.</span><span class="sxs-lookup"><span data-stu-id="f9b54-151">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="f9b54-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9b54-152">userPrincipalName</span></span>|<span data-ttu-id="f9b54-153">String</span><span class="sxs-lookup"><span data-stu-id="f9b54-153">String</span></span>|<span data-ttu-id="f9b54-154">UPN пользователя при записи принятия.</span><span class="sxs-lookup"><span data-stu-id="f9b54-154">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9b54-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="f9b54-155">Relationships</span></span>
<span data-ttu-id="f9b54-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f9b54-156">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f9b54-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f9b54-157">JSON representation</span></span>

<span data-ttu-id="f9b54-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9b54-158">The following is a JSON representation of the resource.</span></span>

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


