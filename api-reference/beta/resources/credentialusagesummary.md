---
title: Тип ресурса credentialUsageSummary
description: Представляет текущее состояние того, сколько пользователей в организации используют возможности самостоятельного сброса паролей.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 03ae7b4b03cf58301895e5246fa4cb86d1b79667
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157703"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="e4060-103">Тип ресурса credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="e4060-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="e4060-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4060-105">Представляет текущее состояние того, сколько пользователей в организации используют возможности самостоятельного сброса паролей.</span><span class="sxs-lookup"><span data-stu-id="e4060-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="e4060-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e4060-106">Methods</span></span>

| <span data-ttu-id="e4060-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e4060-107">Method</span></span>       | <span data-ttu-id="e4060-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4060-108">Return Type</span></span> | <span data-ttu-id="e4060-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4060-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e4060-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="e4060-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="e4060-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="e4060-111">credentialUsageSummary</span></span> | <span data-ttu-id="e4060-112">Чтение свойств и связей объекта credentialUsageSummary.</span><span class="sxs-lookup"><span data-stu-id="e4060-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4060-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4060-113">Properties</span></span>

| <span data-ttu-id="e4060-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4060-114">Property</span></span>     | <span data-ttu-id="e4060-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e4060-115">Type</span></span>        | <span data-ttu-id="e4060-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e4060-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e4060-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="e4060-117">authMethod</span></span> | <span data-ttu-id="e4060-118">string</span><span class="sxs-lookup"><span data-stu-id="e4060-118">string</span></span> | <span data-ttu-id="e4060-119">Представляет метод проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="e4060-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="e4060-120">Возможные значения: , , , , (используется только для самостоятельного сброса `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), `appNotification` , и `appCode`  `alternateMobileCall` (поддерживается только для регистрации).</span><span class="sxs-lookup"><span data-stu-id="e4060-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="e4060-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="e4060-121">failureActivityCount</span></span> | <span data-ttu-id="e4060-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e4060-122">Int64</span></span> | <span data-ttu-id="e4060-123">Предоставляет количество неудачных сбросов или регистрационных данных.</span><span class="sxs-lookup"><span data-stu-id="e4060-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="e4060-124">feature</span><span class="sxs-lookup"><span data-stu-id="e4060-124">feature</span></span> | <span data-ttu-id="e4060-125">string</span><span class="sxs-lookup"><span data-stu-id="e4060-125">string</span></span> | <span data-ttu-id="e4060-126">Определяет функцию для отчета.</span><span class="sxs-lookup"><span data-stu-id="e4060-126">Defines the feature to report.</span></span> <span data-ttu-id="e4060-127">Возможные значения: `registration` и `reset` .</span><span class="sxs-lookup"><span data-stu-id="e4060-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="e4060-128">id</span><span class="sxs-lookup"><span data-stu-id="e4060-128">id</span></span> | <span data-ttu-id="e4060-129">String</span><span class="sxs-lookup"><span data-stu-id="e4060-129">String</span></span> | <span data-ttu-id="e4060-130">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="e4060-130">The unique identifier for the activity.</span></span> <span data-ttu-id="e4060-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e4060-131">Read-only.</span></span> |
| <span data-ttu-id="e4060-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="e4060-132">successfulActivityCount</span></span> | <span data-ttu-id="e4060-133">Int64</span><span class="sxs-lookup"><span data-stu-id="e4060-133">Int64</span></span> | <span data-ttu-id="e4060-134">Предоставляет количество успешных регистраций или сбросов.</span><span class="sxs-lookup"><span data-stu-id="e4060-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e4060-135">Связи</span><span class="sxs-lookup"><span data-stu-id="e4060-135">Relationships</span></span>

<span data-ttu-id="e4060-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4060-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4060-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e4060-137">JSON representation</span></span>

<span data-ttu-id="e4060-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4060-138">The following is a JSON representation of the resource.</span></span>

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

