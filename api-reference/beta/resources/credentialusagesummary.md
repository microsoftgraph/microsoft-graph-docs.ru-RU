---
title: Тип ресурса Кредентиалусажесуммари
description: Представляет текущее состояние того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 46fc3f90b7a7f286d61a324e7b5f439d467a4978
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529192"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="76557-103">Тип ресурса Кредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="76557-103">credentialUsageSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76557-104">Представляет текущее состояние того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="76557-104">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="76557-105">Методы</span><span class="sxs-lookup"><span data-stu-id="76557-105">Methods</span></span>

| <span data-ttu-id="76557-106">Метод</span><span class="sxs-lookup"><span data-stu-id="76557-106">Method</span></span>       | <span data-ttu-id="76557-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="76557-107">Return Type</span></span> | <span data-ttu-id="76557-108">Описание</span><span class="sxs-lookup"><span data-stu-id="76557-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="76557-109">Жеткредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="76557-109">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="76557-110">Кредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="76557-110">credentialUsageSummary</span></span> | <span data-ttu-id="76557-111">Чтение свойств и связей объекта Кредентиалусажесуммари.</span><span class="sxs-lookup"><span data-stu-id="76557-111">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="76557-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="76557-112">Properties</span></span>

| <span data-ttu-id="76557-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="76557-113">Property</span></span>     | <span data-ttu-id="76557-114">Тип</span><span class="sxs-lookup"><span data-stu-id="76557-114">Type</span></span>        | <span data-ttu-id="76557-115">Описание</span><span class="sxs-lookup"><span data-stu-id="76557-115">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="76557-116">Аусмесод</span><span class="sxs-lookup"><span data-stu-id="76557-116">authMethod</span></span> | <span data-ttu-id="76557-117">string</span><span class="sxs-lookup"><span data-stu-id="76557-117">string</span></span> | <span data-ttu-id="76557-118">Представляет способ проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="76557-118">Represents the authentication method that the user used.</span></span> <span data-ttu-id="76557-119">Возможные значения `email`:, `mobileSMS`, `mobileCall` `officePhone`,, `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode`и `alternateMobileCall` (поддерживается только для регистрации).</span><span class="sxs-lookup"><span data-stu-id="76557-119">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="76557-120">Фаилуреактивитикаунт</span><span class="sxs-lookup"><span data-stu-id="76557-120">failureActivityCount</span></span> | <span data-ttu-id="76557-121">Int64</span><span class="sxs-lookup"><span data-stu-id="76557-121">Int64</span></span> | <span data-ttu-id="76557-122">Предоставляет количество неудачных сбросов или регистрационных данных.</span><span class="sxs-lookup"><span data-stu-id="76557-122">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="76557-123">состав</span><span class="sxs-lookup"><span data-stu-id="76557-123">feature</span></span> | <span data-ttu-id="76557-124">string</span><span class="sxs-lookup"><span data-stu-id="76557-124">string</span></span> | <span data-ttu-id="76557-125">Определяет компонент для отчета.</span><span class="sxs-lookup"><span data-stu-id="76557-125">Defines the feature to report.</span></span> <span data-ttu-id="76557-126">Возможные значения: `registration` и `reset`.</span><span class="sxs-lookup"><span data-stu-id="76557-126">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="76557-127">id</span><span class="sxs-lookup"><span data-stu-id="76557-127">id</span></span> | <span data-ttu-id="76557-128">String</span><span class="sxs-lookup"><span data-stu-id="76557-128">String</span></span> | <span data-ttu-id="76557-129">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="76557-129">The unique identifier for the activity.</span></span> <span data-ttu-id="76557-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76557-130">Read-only.</span></span> |
| <span data-ttu-id="76557-131">Сукцессфулактивитикаунт</span><span class="sxs-lookup"><span data-stu-id="76557-131">successfulActivityCount</span></span> | <span data-ttu-id="76557-132">Int64</span><span class="sxs-lookup"><span data-stu-id="76557-132">Int64</span></span> | <span data-ttu-id="76557-133">Предоставляет количество успешных регистраций или сбросов.</span><span class="sxs-lookup"><span data-stu-id="76557-133">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="76557-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="76557-134">Relationships</span></span>

<span data-ttu-id="76557-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="76557-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76557-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="76557-136">JSON representation</span></span>

<span data-ttu-id="76557-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76557-137">The following is a JSON representation of the resource.</span></span>

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