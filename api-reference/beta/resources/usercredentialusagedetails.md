---
title: тип ресурса userCredentialUsageDetails
description: Представляет использование сброса пароля самообслуживателя для данного клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a10d262444b0a33dfbeadbb21611d914d9253e0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719908"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="699de-103">тип ресурса userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="699de-103">userCredentialUsageDetails resource type</span></span>

<span data-ttu-id="699de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="699de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="699de-105">Представляет использование сброса пароля самообслуживателя для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="699de-105">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="699de-106">Сведения включают сведения о пользователях, состояние сброса и причину сбоя.</span><span class="sxs-lookup"><span data-stu-id="699de-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="699de-107">Методы</span><span class="sxs-lookup"><span data-stu-id="699de-107">Methods</span></span>

| <span data-ttu-id="699de-108">Метод</span><span class="sxs-lookup"><span data-stu-id="699de-108">Method</span></span>       | <span data-ttu-id="699de-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="699de-109">Return Type</span></span> | <span data-ttu-id="699de-110">Описание</span><span class="sxs-lookup"><span data-stu-id="699de-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="699de-111">Список пользователейCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="699de-111">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="699de-112">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="699de-112">userCredentialUsageDetails</span></span> | <span data-ttu-id="699de-113">Чтение свойств и связей объекта userCredentialUsageDetails.</span><span class="sxs-lookup"><span data-stu-id="699de-113">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="699de-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="699de-114">Properties</span></span>

| <span data-ttu-id="699de-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="699de-115">Property</span></span>     | <span data-ttu-id="699de-116">Тип</span><span class="sxs-lookup"><span data-stu-id="699de-116">Type</span></span>        | <span data-ttu-id="699de-117">Описание</span><span class="sxs-lookup"><span data-stu-id="699de-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="699de-118">authMethod</span><span class="sxs-lookup"><span data-stu-id="699de-118">authMethod</span></span> | <span data-ttu-id="699de-119">Строка</span><span class="sxs-lookup"><span data-stu-id="699de-119">string</span></span> | <span data-ttu-id="699de-120">Представляет метод проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="699de-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="699de-121">Возможные значения: , , , , (только используется для самообслуживки сброс `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), `appNotification` , и `appCode` `alternateMobileCall` (поддерживается только в регистрации).</span><span class="sxs-lookup"><span data-stu-id="699de-121">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="699de-122">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="699de-122">eventDateTime</span></span> | <span data-ttu-id="699de-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="699de-123">DateTimeOffset</span></span> | <span data-ttu-id="699de-124">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="699de-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="699de-125">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="699de-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="699de-126">failureReason</span><span class="sxs-lookup"><span data-stu-id="699de-126">failureReason</span></span> | <span data-ttu-id="699de-127">String</span><span class="sxs-lookup"><span data-stu-id="699de-127">String</span></span> | <span data-ttu-id="699de-128">Предоставляет причину сбоя для соответствующего рабочего процесса сброса или регистрации.</span><span class="sxs-lookup"><span data-stu-id="699de-128">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="699de-129">функция</span><span class="sxs-lookup"><span data-stu-id="699de-129">feature</span></span> | <span data-ttu-id="699de-130">Строка</span><span class="sxs-lookup"><span data-stu-id="699de-130">string</span></span> | <span data-ttu-id="699de-131">Возможные значения: `registration` и `reset` .</span><span class="sxs-lookup"><span data-stu-id="699de-131">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="699de-132">id</span><span class="sxs-lookup"><span data-stu-id="699de-132">id</span></span> | <span data-ttu-id="699de-133">String</span><span class="sxs-lookup"><span data-stu-id="699de-133">String</span></span> | <span data-ttu-id="699de-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="699de-134">Read-only.</span></span> <span data-ttu-id="699de-135">Уникальный идентификатор для этого действия.</span><span class="sxs-lookup"><span data-stu-id="699de-135">The unique identifier for the activity.</span></span> <span data-ttu-id="699de-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="699de-136">Read-only.</span></span>|
| <span data-ttu-id="699de-137">isSuccess</span><span class="sxs-lookup"><span data-stu-id="699de-137">isSuccess</span></span> | <span data-ttu-id="699de-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="699de-138">Boolean</span></span> | <span data-ttu-id="699de-139">Указывает на успешность или сбой рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="699de-139">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="699de-140">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="699de-140">userDisplayName</span></span> | <span data-ttu-id="699de-141">String</span><span class="sxs-lookup"><span data-stu-id="699de-141">String</span></span> | <span data-ttu-id="699de-142">Имя пользователя, который выполняет рабочий процесс сброса или регистрации.</span><span class="sxs-lookup"><span data-stu-id="699de-142">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="699de-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="699de-143">userPrincipalName</span></span> | <span data-ttu-id="699de-144">String</span><span class="sxs-lookup"><span data-stu-id="699de-144">String</span></span> | <span data-ttu-id="699de-145">Основное имя пользователя, который выполняет рабочий процесс сброса или регистрации.</span><span class="sxs-lookup"><span data-stu-id="699de-145">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="699de-146">Связи</span><span class="sxs-lookup"><span data-stu-id="699de-146">Relationships</span></span>

<span data-ttu-id="699de-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="699de-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="699de-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="699de-148">JSON representation</span></span>

<span data-ttu-id="699de-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="699de-149">The following is a JSON representation of the resource.</span></span>

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

