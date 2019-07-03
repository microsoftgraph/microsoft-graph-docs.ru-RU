---
title: Тип ресурса Усеркредентиалусажедетаилс
description: Представляет использование функции самостоятельного сброса пароля для данного клиента.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: bb92f3bfc91e8fa418d6a33ad6a77a5fddbf9f10
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529737"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="87ffa-103">Тип ресурса Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="87ffa-103">userCredentialUsageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87ffa-104">Представляет использование функции самостоятельного сброса пароля для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="87ffa-104">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="87ffa-105">Сведения включают сведения о пользователе, состояние сброса и причину сбоя.</span><span class="sxs-lookup"><span data-stu-id="87ffa-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="87ffa-106">Методы</span><span class="sxs-lookup"><span data-stu-id="87ffa-106">Methods</span></span>

| <span data-ttu-id="87ffa-107">Метод</span><span class="sxs-lookup"><span data-stu-id="87ffa-107">Method</span></span>       | <span data-ttu-id="87ffa-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="87ffa-108">Return Type</span></span> | <span data-ttu-id="87ffa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87ffa-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="87ffa-110">Список Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="87ffa-110">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="87ffa-111">Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="87ffa-111">userCredentialUsageDetails</span></span> | <span data-ttu-id="87ffa-112">Чтение свойств и связей объекта Усеркредентиалусажедетаилс.</span><span class="sxs-lookup"><span data-stu-id="87ffa-112">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="87ffa-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="87ffa-113">Properties</span></span>

| <span data-ttu-id="87ffa-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="87ffa-114">Property</span></span>     | <span data-ttu-id="87ffa-115">Тип</span><span class="sxs-lookup"><span data-stu-id="87ffa-115">Type</span></span>        | <span data-ttu-id="87ffa-116">Описание</span><span class="sxs-lookup"><span data-stu-id="87ffa-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="87ffa-117">Аусмесод</span><span class="sxs-lookup"><span data-stu-id="87ffa-117">authMethod</span></span> | <span data-ttu-id="87ffa-118">string</span><span class="sxs-lookup"><span data-stu-id="87ffa-118">string</span></span> | <span data-ttu-id="87ffa-119">Представляет способ проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="87ffa-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="87ffa-120">Возможные значения `email`:, `mobileSMS`, `mobileCall` `officePhone`,, `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode`и `alternateMobileCall` (поддерживается только при регистрации).</span><span class="sxs-lookup"><span data-stu-id="87ffa-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="87ffa-121">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="87ffa-121">eventDateTime</span></span> | <span data-ttu-id="87ffa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ffa-122">DateTimeOffset</span></span> | <span data-ttu-id="87ffa-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="87ffa-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87ffa-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="87ffa-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="87ffa-125">failureReason</span><span class="sxs-lookup"><span data-stu-id="87ffa-125">failureReason</span></span> | <span data-ttu-id="87ffa-126">String</span><span class="sxs-lookup"><span data-stu-id="87ffa-126">String</span></span> | <span data-ttu-id="87ffa-127">Предоставляет причину ошибки для соответствующего сброса или рабочего процесса регистрации.</span><span class="sxs-lookup"><span data-stu-id="87ffa-127">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="87ffa-128">состав</span><span class="sxs-lookup"><span data-stu-id="87ffa-128">feature</span></span> | <span data-ttu-id="87ffa-129">string</span><span class="sxs-lookup"><span data-stu-id="87ffa-129">string</span></span> | <span data-ttu-id="87ffa-130">Возможные значения: `registration` и `reset`.</span><span class="sxs-lookup"><span data-stu-id="87ffa-130">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="87ffa-131">id</span><span class="sxs-lookup"><span data-stu-id="87ffa-131">id</span></span> | <span data-ttu-id="87ffa-132">String</span><span class="sxs-lookup"><span data-stu-id="87ffa-132">String</span></span> | <span data-ttu-id="87ffa-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87ffa-133">Read-only.</span></span> <span data-ttu-id="87ffa-134">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="87ffa-134">The unique identifier for the activity.</span></span> <span data-ttu-id="87ffa-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87ffa-135">Read-only.</span></span>|
| <span data-ttu-id="87ffa-136">Выполнение</span><span class="sxs-lookup"><span data-stu-id="87ffa-136">isSuccess</span></span> | <span data-ttu-id="87ffa-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="87ffa-137">Boolean</span></span> | <span data-ttu-id="87ffa-138">Указывает на успешное или неудачное завершение рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="87ffa-138">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="87ffa-139">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="87ffa-139">userDisplayName</span></span> | <span data-ttu-id="87ffa-140">String</span><span class="sxs-lookup"><span data-stu-id="87ffa-140">String</span></span> | <span data-ttu-id="87ffa-141">Имя пользователя, выполняющего сброс или регистрацию рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="87ffa-141">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="87ffa-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="87ffa-142">userPrincipalName</span></span> | <span data-ttu-id="87ffa-143">Строка</span><span class="sxs-lookup"><span data-stu-id="87ffa-143">String</span></span> | <span data-ttu-id="87ffa-144">Имя участника-пользователя, выполняющего сброс или регистрацию.</span><span class="sxs-lookup"><span data-stu-id="87ffa-144">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="87ffa-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="87ffa-145">Relationships</span></span>

<span data-ttu-id="87ffa-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="87ffa-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87ffa-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="87ffa-147">JSON representation</span></span>

<span data-ttu-id="87ffa-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87ffa-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "",
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