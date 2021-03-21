---
title: тип ресурса userCredentialUsageDetails
description: Представляет использование сброса пароля самообслуживателя для данного клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: deb5c93570a9921bc1830bfcb0772d643eed68b7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958733"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="38b6e-103">тип ресурса userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="38b6e-103">userCredentialUsageDetails resource type</span></span>

<span data-ttu-id="38b6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38b6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38b6e-105">Представляет использование сброса пароля самообслуживателя для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="38b6e-105">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="38b6e-106">Сведения включают сведения о пользователях, состояние сброса и причину сбоя.</span><span class="sxs-lookup"><span data-stu-id="38b6e-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="38b6e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="38b6e-107">Methods</span></span>

| <span data-ttu-id="38b6e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="38b6e-108">Method</span></span>       | <span data-ttu-id="38b6e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="38b6e-109">Return Type</span></span> | <span data-ttu-id="38b6e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38b6e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="38b6e-111">Список пользователейCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="38b6e-111">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="38b6e-112">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="38b6e-112">userCredentialUsageDetails</span></span> | <span data-ttu-id="38b6e-113">Чтение свойств и связей объекта userCredentialUsageDetails.</span><span class="sxs-lookup"><span data-stu-id="38b6e-113">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="38b6e-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="38b6e-114">Properties</span></span>

| <span data-ttu-id="38b6e-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="38b6e-115">Property</span></span>     | <span data-ttu-id="38b6e-116">Тип</span><span class="sxs-lookup"><span data-stu-id="38b6e-116">Type</span></span>        | <span data-ttu-id="38b6e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="38b6e-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="38b6e-118">authMethod</span><span class="sxs-lookup"><span data-stu-id="38b6e-118">authMethod</span></span> | <span data-ttu-id="38b6e-119">useAuthMethod</span><span class="sxs-lookup"><span data-stu-id="38b6e-119">usageAuthMethod</span></span> | <span data-ttu-id="38b6e-120">Представляет метод проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="38b6e-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="38b6e-121">Возможные значения: , , , , (только используется для самообслуживки сброс `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), `appNotification` , , ( `appCode` `alternateMobileCall` поддерживается только в регистрации), `fido` , `appPassword` ,`unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="38b6e-121">Possible values are:`email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, `alternateMobileCall` (supported only in registration), `fido`, `appPassword`,`unknownFutureValue`</span></span> |
| <span data-ttu-id="38b6e-122">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="38b6e-122">eventDateTime</span></span> | <span data-ttu-id="38b6e-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38b6e-123">DateTimeOffset</span></span> | <span data-ttu-id="38b6e-124">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="38b6e-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38b6e-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="38b6e-125">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="38b6e-126">failureReason</span><span class="sxs-lookup"><span data-stu-id="38b6e-126">failureReason</span></span> | <span data-ttu-id="38b6e-127">String</span><span class="sxs-lookup"><span data-stu-id="38b6e-127">String</span></span> | <span data-ttu-id="38b6e-128">Предоставляет причину сбоя для соответствующего рабочего процесса сброса или регистрации.</span><span class="sxs-lookup"><span data-stu-id="38b6e-128">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="38b6e-129">функция</span><span class="sxs-lookup"><span data-stu-id="38b6e-129">feature</span></span> | <span data-ttu-id="38b6e-130">featureType</span><span class="sxs-lookup"><span data-stu-id="38b6e-130">featureType</span></span> | <span data-ttu-id="38b6e-131">Возможные значения: `registration`, `reset`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="38b6e-131">Possible values are: `registration`, `reset`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="38b6e-132">id</span><span class="sxs-lookup"><span data-stu-id="38b6e-132">id</span></span> | <span data-ttu-id="38b6e-133">String</span><span class="sxs-lookup"><span data-stu-id="38b6e-133">String</span></span> | <span data-ttu-id="38b6e-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38b6e-134">Read-only.</span></span> <span data-ttu-id="38b6e-135">Уникальный идентификатор для этого действия.</span><span class="sxs-lookup"><span data-stu-id="38b6e-135">The unique identifier for the activity.</span></span> <span data-ttu-id="38b6e-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38b6e-136">Read-only.</span></span>|
| <span data-ttu-id="38b6e-137">isSuccess</span><span class="sxs-lookup"><span data-stu-id="38b6e-137">isSuccess</span></span> | <span data-ttu-id="38b6e-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="38b6e-138">Boolean</span></span> | <span data-ttu-id="38b6e-139">Указывает на успешность или сбой рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="38b6e-139">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="38b6e-140">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="38b6e-140">userDisplayName</span></span> | <span data-ttu-id="38b6e-141">String</span><span class="sxs-lookup"><span data-stu-id="38b6e-141">String</span></span> | <span data-ttu-id="38b6e-142">Имя пользователя, который выполняет рабочий процесс сброса или регистрации.</span><span class="sxs-lookup"><span data-stu-id="38b6e-142">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="38b6e-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38b6e-143">userPrincipalName</span></span> | <span data-ttu-id="38b6e-144">String</span><span class="sxs-lookup"><span data-stu-id="38b6e-144">String</span></span> | <span data-ttu-id="38b6e-145">Основное имя пользователя, который выполняет рабочий процесс сброса или регистрации.</span><span class="sxs-lookup"><span data-stu-id="38b6e-145">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="38b6e-146">Связи</span><span class="sxs-lookup"><span data-stu-id="38b6e-146">Relationships</span></span>

<span data-ttu-id="38b6e-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="38b6e-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38b6e-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="38b6e-148">JSON representation</span></span>

<span data-ttu-id="38b6e-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38b6e-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

