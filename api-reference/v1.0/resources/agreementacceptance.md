---
title: тип ресурса agreementAcceptance
description: Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с использованием Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: ac0e6d67e10e7d7b81fc1c5c21e93251f84cab0a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722794"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="180af-103">тип ресурса agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="180af-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="180af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="180af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="180af-105">Представляет текущее состояние пользователя в пределах настраиваемых условий использования компании с использованием Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="180af-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="180af-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="180af-106">Properties</span></span>
| <span data-ttu-id="180af-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="180af-107">Property</span></span>     | <span data-ttu-id="180af-108">Тип</span><span class="sxs-lookup"><span data-stu-id="180af-108">Type</span></span>        | <span data-ttu-id="180af-109">Описание</span><span class="sxs-lookup"><span data-stu-id="180af-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="180af-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="180af-110">agreementFileId</span></span>|<span data-ttu-id="180af-111">String</span><span class="sxs-lookup"><span data-stu-id="180af-111">String</span></span>|<span data-ttu-id="180af-112">Идентификатор файла соглашения, принятого пользователем.</span><span class="sxs-lookup"><span data-stu-id="180af-112">The identifier of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="180af-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="180af-113">agreementId</span></span>|<span data-ttu-id="180af-114">String</span><span class="sxs-lookup"><span data-stu-id="180af-114">String</span></span>|<span data-ttu-id="180af-115">Идентификатор соглашения.</span><span class="sxs-lookup"><span data-stu-id="180af-115">The identifier of the agreement.</span></span>|
|<span data-ttu-id="180af-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="180af-116">deviceDisplayName</span></span>|<span data-ttu-id="180af-117">String</span><span class="sxs-lookup"><span data-stu-id="180af-117">String</span></span>|<span data-ttu-id="180af-118">Отображающее имя устройства, используемого для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="180af-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="180af-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="180af-119">deviceId</span></span>|<span data-ttu-id="180af-120">String</span><span class="sxs-lookup"><span data-stu-id="180af-120">String</span></span>|<span data-ttu-id="180af-121">Уникальный идентификатор устройства, используемого для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="180af-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="180af-122">deviceOSType</span><span class="sxs-lookup"><span data-stu-id="180af-122">deviceOSType</span></span>|<span data-ttu-id="180af-123">String</span><span class="sxs-lookup"><span data-stu-id="180af-123">String</span></span>|<span data-ttu-id="180af-124">Операционная система, используемая для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="180af-124">The operating system used to accept the agreement.</span></span>|
|<span data-ttu-id="180af-125">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="180af-125">deviceOSVersion</span></span>|<span data-ttu-id="180af-126">String</span><span class="sxs-lookup"><span data-stu-id="180af-126">String</span></span>|<span data-ttu-id="180af-127">Версия операционной системы устройства, используемая для принятие соглашения.</span><span class="sxs-lookup"><span data-stu-id="180af-127">The operating system version of the device used to accept the agreement.</span></span>    |
|<span data-ttu-id="180af-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="180af-128">expirationDateTime</span></span>|<span data-ttu-id="180af-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180af-129">DateTimeOffset</span></span>|<span data-ttu-id="180af-130">Срок действия даты принятия.</span><span class="sxs-lookup"><span data-stu-id="180af-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="180af-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="180af-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="180af-132">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="180af-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="180af-133">id</span><span class="sxs-lookup"><span data-stu-id="180af-133">id</span></span>|<span data-ttu-id="180af-134">String</span><span class="sxs-lookup"><span data-stu-id="180af-134">String</span></span>| <span data-ttu-id="180af-135">Идентификатор принятия соглашения.</span><span class="sxs-lookup"><span data-stu-id="180af-135">The identifier of the agreement acceptance.</span></span> <span data-ttu-id="180af-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="180af-136">Read-only.</span></span>|
|<span data-ttu-id="180af-137">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="180af-137">recordedDateTime</span></span>|<span data-ttu-id="180af-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180af-138">DateTimeOffset</span></span>|<span data-ttu-id="180af-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="180af-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="180af-141">состояние</span><span class="sxs-lookup"><span data-stu-id="180af-141">state</span></span>|<span data-ttu-id="180af-142">string</span><span class="sxs-lookup"><span data-stu-id="180af-142">string</span></span>| <span data-ttu-id="180af-143">Состояние принятия соглашения.</span><span class="sxs-lookup"><span data-stu-id="180af-143">The state of the agreement acceptance.</span></span> <span data-ttu-id="180af-144">Возможные значения: `accepted`, `declined`.</span><span class="sxs-lookup"><span data-stu-id="180af-144">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="180af-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="180af-145">userDisplayName</span></span>|<span data-ttu-id="180af-146">String</span><span class="sxs-lookup"><span data-stu-id="180af-146">String</span></span>|<span data-ttu-id="180af-147">Отображение имени пользователя при записи приемки.</span><span class="sxs-lookup"><span data-stu-id="180af-147">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="180af-148">userEmail</span><span class="sxs-lookup"><span data-stu-id="180af-148">userEmail</span></span>|<span data-ttu-id="180af-149">String</span><span class="sxs-lookup"><span data-stu-id="180af-149">String</span></span>|<span data-ttu-id="180af-150">Электронная почта пользователя при записи принятия.</span><span class="sxs-lookup"><span data-stu-id="180af-150">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="180af-151">userId</span><span class="sxs-lookup"><span data-stu-id="180af-151">userId</span></span>|<span data-ttu-id="180af-152">String</span><span class="sxs-lookup"><span data-stu-id="180af-152">String</span></span>|<span data-ttu-id="180af-153">Идентификатор пользователя, который принял соглашение.</span><span class="sxs-lookup"><span data-stu-id="180af-153">The identifier of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="180af-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="180af-154">userPrincipalName</span></span>|<span data-ttu-id="180af-155">String</span><span class="sxs-lookup"><span data-stu-id="180af-155">String</span></span>|<span data-ttu-id="180af-156">UPN пользователя при записи принятия.</span><span class="sxs-lookup"><span data-stu-id="180af-156">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="180af-157">Связи</span><span class="sxs-lookup"><span data-stu-id="180af-157">Relationships</span></span>
<span data-ttu-id="180af-158">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="180af-158">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="180af-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="180af-159">JSON representation</span></span>

<span data-ttu-id="180af-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="180af-160">The following is a JSON representation of the resource.</span></span>

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


