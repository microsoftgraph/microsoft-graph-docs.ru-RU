---
title: Тип ресурса Кредентиалусажесуммари
description: Представляет текущее состояние того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 17fc4535e5132b6bf6c2f6eab4a94b5a58ef9bb1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507354"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="cbed2-103">Тип ресурса Кредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="cbed2-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="cbed2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cbed2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbed2-105">Представляет текущее состояние того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="cbed2-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="cbed2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cbed2-106">Methods</span></span>

| <span data-ttu-id="cbed2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cbed2-107">Method</span></span>       | <span data-ttu-id="cbed2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cbed2-108">Return Type</span></span> | <span data-ttu-id="cbed2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cbed2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cbed2-110">жеткредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="cbed2-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="cbed2-111">кредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="cbed2-111">credentialUsageSummary</span></span> | <span data-ttu-id="cbed2-112">Чтение свойств и связей объекта Кредентиалусажесуммари.</span><span class="sxs-lookup"><span data-stu-id="cbed2-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cbed2-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbed2-113">Properties</span></span>

| <span data-ttu-id="cbed2-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbed2-114">Property</span></span>     | <span data-ttu-id="cbed2-115">Тип</span><span class="sxs-lookup"><span data-stu-id="cbed2-115">Type</span></span>        | <span data-ttu-id="cbed2-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cbed2-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cbed2-117">аусмесод</span><span class="sxs-lookup"><span data-stu-id="cbed2-117">authMethod</span></span> | <span data-ttu-id="cbed2-118">строка</span><span class="sxs-lookup"><span data-stu-id="cbed2-118">string</span></span> | <span data-ttu-id="cbed2-119">Представляет способ проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="cbed2-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="cbed2-120">Возможные значения `email`:, `mobileSMS`, `mobileCall` `officePhone`,, `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode`и `alternateMobileCall` (поддерживается только для регистрации).</span><span class="sxs-lookup"><span data-stu-id="cbed2-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="cbed2-121">фаилуреактивитикаунт</span><span class="sxs-lookup"><span data-stu-id="cbed2-121">failureActivityCount</span></span> | <span data-ttu-id="cbed2-122">Int64</span><span class="sxs-lookup"><span data-stu-id="cbed2-122">Int64</span></span> | <span data-ttu-id="cbed2-123">Предоставляет количество неудачных сбросов или регистрационных данных.</span><span class="sxs-lookup"><span data-stu-id="cbed2-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="cbed2-124">состав</span><span class="sxs-lookup"><span data-stu-id="cbed2-124">feature</span></span> | <span data-ttu-id="cbed2-125">строка</span><span class="sxs-lookup"><span data-stu-id="cbed2-125">string</span></span> | <span data-ttu-id="cbed2-126">Определяет компонент для отчета.</span><span class="sxs-lookup"><span data-stu-id="cbed2-126">Defines the feature to report.</span></span> <span data-ttu-id="cbed2-127">Возможные значения: `registration` и `reset`.</span><span class="sxs-lookup"><span data-stu-id="cbed2-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="cbed2-128">id</span><span class="sxs-lookup"><span data-stu-id="cbed2-128">id</span></span> | <span data-ttu-id="cbed2-129">String</span><span class="sxs-lookup"><span data-stu-id="cbed2-129">String</span></span> | <span data-ttu-id="cbed2-130">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="cbed2-130">The unique identifier for the activity.</span></span> <span data-ttu-id="cbed2-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cbed2-131">Read-only.</span></span> |
| <span data-ttu-id="cbed2-132">сукцессфулактивитикаунт</span><span class="sxs-lookup"><span data-stu-id="cbed2-132">successfulActivityCount</span></span> | <span data-ttu-id="cbed2-133">Int64</span><span class="sxs-lookup"><span data-stu-id="cbed2-133">Int64</span></span> | <span data-ttu-id="cbed2-134">Предоставляет количество успешных регистраций или сбросов.</span><span class="sxs-lookup"><span data-stu-id="cbed2-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cbed2-135">Связи</span><span class="sxs-lookup"><span data-stu-id="cbed2-135">Relationships</span></span>

<span data-ttu-id="cbed2-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cbed2-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbed2-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cbed2-137">JSON representation</span></span>

<span data-ttu-id="cbed2-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbed2-138">The following is a JSON representation of the resource.</span></span>

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