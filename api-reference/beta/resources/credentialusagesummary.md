---
title: тип ресурса credentialUsageSummary
description: Представляет текущее состояние того, сколько пользователей в организации используют возможности сброса паролей самообслуживки.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9db31a0d0397f1394a342fb52796a1bec37bae36
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941832"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="57597-103">тип ресурса credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="57597-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="57597-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57597-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57597-105">Представляет текущее состояние того, сколько пользователей в организации используют возможности сброса паролей самообслуживки.</span><span class="sxs-lookup"><span data-stu-id="57597-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="57597-106">Методы</span><span class="sxs-lookup"><span data-stu-id="57597-106">Methods</span></span>

| <span data-ttu-id="57597-107">Метод</span><span class="sxs-lookup"><span data-stu-id="57597-107">Method</span></span>       | <span data-ttu-id="57597-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="57597-108">Return Type</span></span> | <span data-ttu-id="57597-109">Описание</span><span class="sxs-lookup"><span data-stu-id="57597-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="57597-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="57597-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="57597-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="57597-111">credentialUsageSummary</span></span> | <span data-ttu-id="57597-112">Чтение свойств и связей объекта credentialUsageSummary.</span><span class="sxs-lookup"><span data-stu-id="57597-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="57597-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="57597-113">Properties</span></span>

| <span data-ttu-id="57597-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="57597-114">Property</span></span>     | <span data-ttu-id="57597-115">Тип</span><span class="sxs-lookup"><span data-stu-id="57597-115">Type</span></span>        | <span data-ttu-id="57597-116">Описание</span><span class="sxs-lookup"><span data-stu-id="57597-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="57597-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="57597-117">authMethod</span></span> | <span data-ttu-id="57597-118">useAuthMethod</span><span class="sxs-lookup"><span data-stu-id="57597-118">usageAuthMethod</span></span> | <span data-ttu-id="57597-119">Представляет метод проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="57597-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="57597-120">Возможные значения: , , , , (только используется для самообслуживки сброс `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), , , ( `appNotification` `appCode` `alternateMobileCall` поддерживается `fido` `appPassword` `unknownFutureValue` только в регистрации), , , .</span><span class="sxs-lookup"><span data-stu-id="57597-120">Possible values are:`email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, `alternateMobileCall` (supported only in registration), `fido`, `appPassword`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="57597-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="57597-121">failureActivityCount</span></span> | <span data-ttu-id="57597-122">Int64</span><span class="sxs-lookup"><span data-stu-id="57597-122">Int64</span></span> | <span data-ttu-id="57597-123">Обеспечивает количество сбойных сбросов или данных регистрации.</span><span class="sxs-lookup"><span data-stu-id="57597-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="57597-124">функция</span><span class="sxs-lookup"><span data-stu-id="57597-124">feature</span></span> | <span data-ttu-id="57597-125">featureType</span><span class="sxs-lookup"><span data-stu-id="57597-125">featureType</span></span> | <span data-ttu-id="57597-126">Определяет функцию для отчета.</span><span class="sxs-lookup"><span data-stu-id="57597-126">Defines the feature to report.</span></span> <span data-ttu-id="57597-127">Возможные значения: `registration`, `reset`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="57597-127">Possible values are: `registration`, `reset`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="57597-128">id</span><span class="sxs-lookup"><span data-stu-id="57597-128">id</span></span> | <span data-ttu-id="57597-129">Строка</span><span class="sxs-lookup"><span data-stu-id="57597-129">String</span></span> | <span data-ttu-id="57597-130">Уникальный идентификатор для этого действия.</span><span class="sxs-lookup"><span data-stu-id="57597-130">The unique identifier for the activity.</span></span> <span data-ttu-id="57597-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57597-131">Read-only.</span></span> |
| <span data-ttu-id="57597-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="57597-132">successfulActivityCount</span></span> | <span data-ttu-id="57597-133">Int64</span><span class="sxs-lookup"><span data-stu-id="57597-133">Int64</span></span> | <span data-ttu-id="57597-134">Обеспечивает количество успешных регистраций или сбросов.</span><span class="sxs-lookup"><span data-stu-id="57597-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="57597-135">Связи</span><span class="sxs-lookup"><span data-stu-id="57597-135">Relationships</span></span>

<span data-ttu-id="57597-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="57597-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57597-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="57597-137">JSON representation</span></span>

<span data-ttu-id="57597-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57597-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "successfulActivityCount":"Int64",
  "failureActivityCount": "Int64",
  "authMethod": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUsageSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

