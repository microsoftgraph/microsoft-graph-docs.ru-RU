---
title: тип ресурса relyingPartyDetailedSummary
description: Представляет надеющийся участник в AD FS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6e840c47ed5170f95929d686fe9ff94be54ea1ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962114"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="23961-103">тип ресурса relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="23961-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="23961-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23961-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23961-105">Представляет доверяемую сторону, настроенную с помощью служб Федерации Active Directory (AD FS), ее агрегированное использование и возможность переноса конфигурации доверяющих сторон в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="23961-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="23961-106">Методы</span><span class="sxs-lookup"><span data-stu-id="23961-106">Methods</span></span>

| <span data-ttu-id="23961-107">Метод</span><span class="sxs-lookup"><span data-stu-id="23961-107">Method</span></span>       | <span data-ttu-id="23961-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="23961-108">Return Type</span></span> | <span data-ttu-id="23961-109">Описание</span><span class="sxs-lookup"><span data-stu-id="23961-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="23961-110">Список</span><span class="sxs-lookup"><span data-stu-id="23961-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="23961-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="23961-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="23961-112">Извлечение списка **объектов relyingPartyDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="23961-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="23961-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="23961-113">Properties</span></span>

| <span data-ttu-id="23961-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="23961-114">Property</span></span>     | <span data-ttu-id="23961-115">Тип</span><span class="sxs-lookup"><span data-stu-id="23961-115">Type</span></span>        | <span data-ttu-id="23961-116">Описание</span><span class="sxs-lookup"><span data-stu-id="23961-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23961-117">id</span><span class="sxs-lookup"><span data-stu-id="23961-117">id</span></span>|<span data-ttu-id="23961-118">String</span><span class="sxs-lookup"><span data-stu-id="23961-118">String</span></span>| <span data-ttu-id="23961-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23961-119">Read-only.</span></span> <span data-ttu-id="23961-120">Уникальный идентификатор, созданный на уровне API.</span><span class="sxs-lookup"><span data-stu-id="23961-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="23961-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="23961-121">relyingPartyId</span></span>|<span data-ttu-id="23961-122">Строка</span><span class="sxs-lookup"><span data-stu-id="23961-122">String</span></span>|<span data-ttu-id="23961-123">Этот идентификатор используется для идентификации сторон, которые полагаются на эту службу Федерации.</span><span class="sxs-lookup"><span data-stu-id="23961-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="23961-124">Он используется при выдаче утверждений стороне, которая полагается.</span><span class="sxs-lookup"><span data-stu-id="23961-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="23961-125">serviceId</span><span class="sxs-lookup"><span data-stu-id="23961-125">serviceId</span></span>|<span data-ttu-id="23961-126">Строка</span><span class="sxs-lookup"><span data-stu-id="23961-126">String</span></span>|<span data-ttu-id="23961-127">Уникально определяет лес Active Directory.</span><span class="sxs-lookup"><span data-stu-id="23961-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="23961-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="23961-128">migrationStatus</span></span>|<span data-ttu-id="23961-129">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="23961-129">migrationStatus</span></span>| <span data-ttu-id="23961-130">Указание на возможность перемещений приложения в Azure AD или требуется дополнительное исследование.</span><span class="sxs-lookup"><span data-stu-id="23961-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="23961-131">Возможные значения: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="23961-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="23961-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="23961-132">migrationValidationDetails</span></span>|<span data-ttu-id="23961-133">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="23961-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="23961-134">Указывает все проверки проверки, которые были сделаны в сведениях о конфигурации приложений, чтобы оценить, готово ли приложение к перемещению в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="23961-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span>|
|<span data-ttu-id="23961-135">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="23961-135">relyingPartyName</span></span>|<span data-ttu-id="23961-136">Строка</span><span class="sxs-lookup"><span data-stu-id="23961-136">String</span></span>|<span data-ttu-id="23961-137">Имя приложения или другого объекта в Интернете, использующего поставщика удостоверений для проверки подлинности пользователя, который хочет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="23961-137">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="23961-138">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="23961-138">failedSignInCount</span></span>|<span data-ttu-id="23961-139">Int64</span><span class="sxs-lookup"><span data-stu-id="23961-139">Int64</span></span>| <span data-ttu-id="23961-140">Количество сбойных входов в службу Федерации Active Directory за указанный период.</span><span class="sxs-lookup"><span data-stu-id="23961-140">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="23961-141">replyUrls</span><span class="sxs-lookup"><span data-stu-id="23961-141">replyUrls</span></span>|<span data-ttu-id="23961-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="23961-142">String collection</span></span>|<span data-ttu-id="23961-143">Указывает, где надеющийся участник ожидает получения маркера.</span><span class="sxs-lookup"><span data-stu-id="23961-143">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="23961-144">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="23961-144">signInSuccessRate</span></span>|<span data-ttu-id="23961-145">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="23961-145">Double</span></span>|<span data-ttu-id="23961-146">Количество успешных / (количество успешных и количество неудачных входов) в службе Федерации Active Directory за указанный период.</span><span class="sxs-lookup"><span data-stu-id="23961-146">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="23961-147">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="23961-147">successfulSignInCount</span></span>|<span data-ttu-id="23961-148">Int64</span><span class="sxs-lookup"><span data-stu-id="23961-148">Int64</span></span>|<span data-ttu-id="23961-149">Количество успешных входов в службу Федерации Active Directory.</span><span class="sxs-lookup"><span data-stu-id="23961-149">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="23961-150">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="23961-150">totalSignInCount</span></span>|<span data-ttu-id="23961-151">Int64</span><span class="sxs-lookup"><span data-stu-id="23961-151">Int64</span></span>|<span data-ttu-id="23961-152">Количество неудачных входов с неудачным входом в службу Федерации Active Directory в указанный период.</span><span class="sxs-lookup"><span data-stu-id="23961-152">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="23961-153">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="23961-153">uniqueUserCount</span></span>|<span data-ttu-id="23961-154">Int64</span><span class="sxs-lookup"><span data-stu-id="23961-154">Int64</span></span>|<span data-ttu-id="23961-155">Количество уникальных пользователей, которые вписались в приложение.</span><span class="sxs-lookup"><span data-stu-id="23961-155">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23961-156">Связи</span><span class="sxs-lookup"><span data-stu-id="23961-156">Relationships</span></span>

<span data-ttu-id="23961-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23961-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23961-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="23961-158">JSON representation</span></span>

<span data-ttu-id="23961-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23961-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "keyProperty": "id"
}-->

```json
{
  "failedSignInCount": 10,
  "id": "String (identifier)",
  "migrationStatus": "ready | needsReview | additionalStepsRequired",
  "migrationValidationDetails": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "relyingPartyId": "String",
  "relyingPartyName": "String",
  "replyUrls": ["String"],
  "serviceId": "String (identifier)",
  "signInSuccessRate": 90.0,
  "successfulSignInCount": 90,
  "totalSignInCount": 100,
  "uniqueUserCount": 10
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relyingPartyDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


