---
title: Тип ресурса Кредентиалусажесуммари
description: Представляет текущее состояние того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 9807e333fd13443462d2d3237150820afd254baa
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523156"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="e82ce-103">Тип ресурса Кредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="e82ce-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="e82ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e82ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e82ce-105">Представляет текущее состояние того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="e82ce-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="e82ce-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e82ce-106">Methods</span></span>

| <span data-ttu-id="e82ce-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e82ce-107">Method</span></span>       | <span data-ttu-id="e82ce-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e82ce-108">Return Type</span></span> | <span data-ttu-id="e82ce-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e82ce-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e82ce-110">жеткредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="e82ce-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="e82ce-111">кредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="e82ce-111">credentialUsageSummary</span></span> | <span data-ttu-id="e82ce-112">Чтение свойств и связей объекта Кредентиалусажесуммари.</span><span class="sxs-lookup"><span data-stu-id="e82ce-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e82ce-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e82ce-113">Properties</span></span>

| <span data-ttu-id="e82ce-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e82ce-114">Property</span></span>     | <span data-ttu-id="e82ce-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e82ce-115">Type</span></span>        | <span data-ttu-id="e82ce-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e82ce-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e82ce-117">аусмесод</span><span class="sxs-lookup"><span data-stu-id="e82ce-117">authMethod</span></span> | <span data-ttu-id="e82ce-118">string</span><span class="sxs-lookup"><span data-stu-id="e82ce-118">string</span></span> | <span data-ttu-id="e82ce-119">Представляет способ проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="e82ce-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="e82ce-120">Возможные значения: `email` ,,,, `mobileSMS` `mobileCall` `officePhone` `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode` и  `alternateMobileCall` (поддерживается только для регистрации).</span><span class="sxs-lookup"><span data-stu-id="e82ce-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="e82ce-121">фаилуреактивитикаунт</span><span class="sxs-lookup"><span data-stu-id="e82ce-121">failureActivityCount</span></span> | <span data-ttu-id="e82ce-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e82ce-122">Int64</span></span> | <span data-ttu-id="e82ce-123">Предоставляет количество неудачных сбросов или регистрационных данных.</span><span class="sxs-lookup"><span data-stu-id="e82ce-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="e82ce-124">состав</span><span class="sxs-lookup"><span data-stu-id="e82ce-124">feature</span></span> | <span data-ttu-id="e82ce-125">string</span><span class="sxs-lookup"><span data-stu-id="e82ce-125">string</span></span> | <span data-ttu-id="e82ce-126">Определяет компонент для отчета.</span><span class="sxs-lookup"><span data-stu-id="e82ce-126">Defines the feature to report.</span></span> <span data-ttu-id="e82ce-127">Возможные значения: `registration` и `reset` .</span><span class="sxs-lookup"><span data-stu-id="e82ce-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="e82ce-128">id</span><span class="sxs-lookup"><span data-stu-id="e82ce-128">id</span></span> | <span data-ttu-id="e82ce-129">String</span><span class="sxs-lookup"><span data-stu-id="e82ce-129">String</span></span> | <span data-ttu-id="e82ce-130">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="e82ce-130">The unique identifier for the activity.</span></span> <span data-ttu-id="e82ce-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e82ce-131">Read-only.</span></span> |
| <span data-ttu-id="e82ce-132">сукцессфулактивитикаунт</span><span class="sxs-lookup"><span data-stu-id="e82ce-132">successfulActivityCount</span></span> | <span data-ttu-id="e82ce-133">Int64</span><span class="sxs-lookup"><span data-stu-id="e82ce-133">Int64</span></span> | <span data-ttu-id="e82ce-134">Предоставляет количество успешных регистраций или сбросов.</span><span class="sxs-lookup"><span data-stu-id="e82ce-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e82ce-135">Связи</span><span class="sxs-lookup"><span data-stu-id="e82ce-135">Relationships</span></span>

<span data-ttu-id="e82ce-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e82ce-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e82ce-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e82ce-137">JSON representation</span></span>

<span data-ttu-id="e82ce-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e82ce-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "",
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

