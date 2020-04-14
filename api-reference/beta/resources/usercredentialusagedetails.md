---
title: Тип ресурса Усеркредентиалусажедетаилс
description: Представляет использование функции самостоятельного сброса пароля для данного клиента.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 9ff48554c7bab011171136181c7a1ab0ce8b01db
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384984"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="ecf34-103">Тип ресурса Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="ecf34-103">userCredentialUsageDetails resource type</span></span>

<span data-ttu-id="ecf34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecf34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecf34-105">Представляет использование функции самостоятельного сброса пароля для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="ecf34-105">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="ecf34-106">Сведения включают сведения о пользователе, состояние сброса и причину сбоя.</span><span class="sxs-lookup"><span data-stu-id="ecf34-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="ecf34-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ecf34-107">Methods</span></span>

| <span data-ttu-id="ecf34-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ecf34-108">Method</span></span>       | <span data-ttu-id="ecf34-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ecf34-109">Return Type</span></span> | <span data-ttu-id="ecf34-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ecf34-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ecf34-111">Список Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="ecf34-111">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="ecf34-112">усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="ecf34-112">userCredentialUsageDetails</span></span> | <span data-ttu-id="ecf34-113">Чтение свойств и связей объекта Усеркредентиалусажедетаилс.</span><span class="sxs-lookup"><span data-stu-id="ecf34-113">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ecf34-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="ecf34-114">Properties</span></span>

| <span data-ttu-id="ecf34-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecf34-115">Property</span></span>     | <span data-ttu-id="ecf34-116">Тип</span><span class="sxs-lookup"><span data-stu-id="ecf34-116">Type</span></span>        | <span data-ttu-id="ecf34-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ecf34-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ecf34-118">аусмесод</span><span class="sxs-lookup"><span data-stu-id="ecf34-118">authMethod</span></span> | <span data-ttu-id="ecf34-119">string</span><span class="sxs-lookup"><span data-stu-id="ecf34-119">string</span></span> | <span data-ttu-id="ecf34-120">Представляет способ проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="ecf34-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="ecf34-121">Возможные значения `email`:, `mobileSMS`, `mobileCall` `officePhone`,, `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode`и `alternateMobileCall` (поддерживается только при регистрации).</span><span class="sxs-lookup"><span data-stu-id="ecf34-121">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="ecf34-122">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="ecf34-122">eventDateTime</span></span> | <span data-ttu-id="ecf34-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecf34-123">DateTimeOffset</span></span> | <span data-ttu-id="ecf34-124">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ecf34-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ecf34-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ecf34-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="ecf34-126">failureReason</span><span class="sxs-lookup"><span data-stu-id="ecf34-126">failureReason</span></span> | <span data-ttu-id="ecf34-127">String</span><span class="sxs-lookup"><span data-stu-id="ecf34-127">String</span></span> | <span data-ttu-id="ecf34-128">Предоставляет причину ошибки для соответствующего сброса или рабочего процесса регистрации.</span><span class="sxs-lookup"><span data-stu-id="ecf34-128">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="ecf34-129">состав</span><span class="sxs-lookup"><span data-stu-id="ecf34-129">feature</span></span> | <span data-ttu-id="ecf34-130">string</span><span class="sxs-lookup"><span data-stu-id="ecf34-130">string</span></span> | <span data-ttu-id="ecf34-131">Возможные значения: `registration` и `reset`.</span><span class="sxs-lookup"><span data-stu-id="ecf34-131">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="ecf34-132">id</span><span class="sxs-lookup"><span data-stu-id="ecf34-132">id</span></span> | <span data-ttu-id="ecf34-133">String</span><span class="sxs-lookup"><span data-stu-id="ecf34-133">String</span></span> | <span data-ttu-id="ecf34-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ecf34-134">Read-only.</span></span> <span data-ttu-id="ecf34-135">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="ecf34-135">The unique identifier for the activity.</span></span> <span data-ttu-id="ecf34-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ecf34-136">Read-only.</span></span>|
| <span data-ttu-id="ecf34-137">Выполнение</span><span class="sxs-lookup"><span data-stu-id="ecf34-137">isSuccess</span></span> | <span data-ttu-id="ecf34-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="ecf34-138">Boolean</span></span> | <span data-ttu-id="ecf34-139">Указывает на успешное или неудачное завершение рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="ecf34-139">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="ecf34-140">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ecf34-140">userDisplayName</span></span> | <span data-ttu-id="ecf34-141">String</span><span class="sxs-lookup"><span data-stu-id="ecf34-141">String</span></span> | <span data-ttu-id="ecf34-142">Имя пользователя, выполняющего сброс или регистрацию рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="ecf34-142">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="ecf34-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ecf34-143">userPrincipalName</span></span> | <span data-ttu-id="ecf34-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ecf34-144">String</span></span> | <span data-ttu-id="ecf34-145">Имя участника-пользователя, выполняющего сброс или регистрацию.</span><span class="sxs-lookup"><span data-stu-id="ecf34-145">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ecf34-146">Связи</span><span class="sxs-lookup"><span data-stu-id="ecf34-146">Relationships</span></span>

<span data-ttu-id="ecf34-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ecf34-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ecf34-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ecf34-148">JSON representation</span></span>

<span data-ttu-id="ecf34-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecf34-149">The following is a JSON representation of the resource.</span></span>

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