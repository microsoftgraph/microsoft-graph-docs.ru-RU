---
title: Тип ресурса credentialUsageSummary
description: Представляет текущее состояние того, сколько пользователей в организации используют возможности самостоятельного сброса паролей.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 43a17f91a1424d9ac8c0a388ef5404bbadf05189
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136286"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="2e461-103">Тип ресурса credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="2e461-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="2e461-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e461-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e461-105">Представляет текущее состояние того, сколько пользователей в организации используют возможности самостоятельного сброса паролей.</span><span class="sxs-lookup"><span data-stu-id="2e461-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="2e461-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2e461-106">Methods</span></span>

| <span data-ttu-id="2e461-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2e461-107">Method</span></span>       | <span data-ttu-id="2e461-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2e461-108">Return Type</span></span> | <span data-ttu-id="2e461-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2e461-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2e461-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="2e461-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="2e461-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="2e461-111">credentialUsageSummary</span></span> | <span data-ttu-id="2e461-112">Чтение свойств и связей объекта credentialUsageSummary.</span><span class="sxs-lookup"><span data-stu-id="2e461-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2e461-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e461-113">Properties</span></span>

| <span data-ttu-id="2e461-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e461-114">Property</span></span>     | <span data-ttu-id="2e461-115">Тип</span><span class="sxs-lookup"><span data-stu-id="2e461-115">Type</span></span>        | <span data-ttu-id="2e461-116">Описание</span><span class="sxs-lookup"><span data-stu-id="2e461-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2e461-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="2e461-117">authMethod</span></span> | <span data-ttu-id="2e461-118">string</span><span class="sxs-lookup"><span data-stu-id="2e461-118">string</span></span> | <span data-ttu-id="2e461-119">Представляет метод проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="2e461-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="2e461-120">Возможные значения: , , , , (используется только для самостоятельного сброса `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), `appNotification` , и `appCode`  `alternateMobileCall` (поддерживается только для регистрации).</span><span class="sxs-lookup"><span data-stu-id="2e461-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="2e461-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="2e461-121">failureActivityCount</span></span> | <span data-ttu-id="2e461-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2e461-122">Int64</span></span> | <span data-ttu-id="2e461-123">Предоставляет количество неудачных сбросов или регистрационных данных.</span><span class="sxs-lookup"><span data-stu-id="2e461-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="2e461-124">feature</span><span class="sxs-lookup"><span data-stu-id="2e461-124">feature</span></span> | <span data-ttu-id="2e461-125">string</span><span class="sxs-lookup"><span data-stu-id="2e461-125">string</span></span> | <span data-ttu-id="2e461-126">Определяет функцию для отчета.</span><span class="sxs-lookup"><span data-stu-id="2e461-126">Defines the feature to report.</span></span> <span data-ttu-id="2e461-127">Возможные значения: `registration` и `reset` .</span><span class="sxs-lookup"><span data-stu-id="2e461-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="2e461-128">id</span><span class="sxs-lookup"><span data-stu-id="2e461-128">id</span></span> | <span data-ttu-id="2e461-129">Строка</span><span class="sxs-lookup"><span data-stu-id="2e461-129">String</span></span> | <span data-ttu-id="2e461-130">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="2e461-130">The unique identifier for the activity.</span></span> <span data-ttu-id="2e461-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e461-131">Read-only.</span></span> |
| <span data-ttu-id="2e461-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="2e461-132">successfulActivityCount</span></span> | <span data-ttu-id="2e461-133">Int64</span><span class="sxs-lookup"><span data-stu-id="2e461-133">Int64</span></span> | <span data-ttu-id="2e461-134">Предоставляет количество успешных регистраций или сбросов.</span><span class="sxs-lookup"><span data-stu-id="2e461-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2e461-135">Связи</span><span class="sxs-lookup"><span data-stu-id="2e461-135">Relationships</span></span>

<span data-ttu-id="2e461-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2e461-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e461-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2e461-137">JSON representation</span></span>

<span data-ttu-id="2e461-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e461-138">The following is a JSON representation of the resource.</span></span>

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

