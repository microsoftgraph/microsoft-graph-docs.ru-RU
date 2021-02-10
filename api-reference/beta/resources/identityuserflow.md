---
title: Тип ресурса UserFlow
description: Потоки пользователей удостоверений — это встроенные пути проверки подлинности
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa6829d346fc1e2520fb5eab28f5ce5fd9c72ae4
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176971"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="4ecc1-103">Тип ресурса UserFlow</span><span class="sxs-lookup"><span data-stu-id="4ecc1-103">UserFlow resource type</span></span>

<span data-ttu-id="4ecc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ecc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ecc1-105">Потоки пользователей позволяют определять предварительно определенные настраиваемые политики для регистрации, регистрации, объединенной регистрации и входов, сброса пароля и обновления профиля.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="4ecc1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4ecc1-106">Methods</span></span>

| <span data-ttu-id="4ecc1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4ecc1-107">Method</span></span>       | <span data-ttu-id="4ecc1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ecc1-108">Return Type</span></span> | <span data-ttu-id="4ecc1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4ecc1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4ecc1-110">Список</span><span class="sxs-lookup"><span data-stu-id="4ecc1-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="4ecc1-111">[Коллекция UserFlow](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="4ecc1-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="4ecc1-112">Список userFlows.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-112">List UserFlows.</span></span> |
| [<span data-ttu-id="4ecc1-113">Создание</span><span class="sxs-lookup"><span data-stu-id="4ecc1-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="4ecc1-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="4ecc1-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="4ecc1-115">Создание объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="4ecc1-116">Получение</span><span class="sxs-lookup"><span data-stu-id="4ecc1-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="4ecc1-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="4ecc1-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="4ecc1-118">Чтение свойств и связей объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-118">Read properties and relationships of UserFlow object.</span></span> |
| <span data-ttu-id="4ecc1-119">[удаление](../api/identityuserflow-delete.md);</span><span class="sxs-lookup"><span data-stu-id="4ecc1-119">[Delete](../api/identityuserflow-delete.md)</span></span> | <span data-ttu-id="4ecc1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4ecc1-120">None</span></span> | <span data-ttu-id="4ecc1-121">Удаление объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4ecc1-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ecc1-122">Properties</span></span>

| <span data-ttu-id="4ecc1-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ecc1-123">Property</span></span>     | <span data-ttu-id="4ecc1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="4ecc1-124">Type</span></span>        | <span data-ttu-id="4ecc1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4ecc1-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4ecc1-126">id</span><span class="sxs-lookup"><span data-stu-id="4ecc1-126">id</span></span>|<span data-ttu-id="4ecc1-127">String</span><span class="sxs-lookup"><span data-stu-id="4ecc1-127">String</span></span>| <span data-ttu-id="4ecc1-128">Идентификатор пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-128">The identifier of the user flow.</span></span> <span data-ttu-id="4ecc1-129">Префикс B2C_1_ **добавляется** к заранее заранее предоставляемого значения.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-129">The prefix of **B2C_1_** is added to the value that you provide.</span></span>|
|<span data-ttu-id="4ecc1-130">userFlowType</span><span class="sxs-lookup"><span data-stu-id="4ecc1-130">userFlowType</span></span>|<span data-ttu-id="4ecc1-131">string</span><span class="sxs-lookup"><span data-stu-id="4ecc1-131">string</span></span>| <span data-ttu-id="4ecc1-132">Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-132">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4ecc1-133">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="4ecc1-133">userFlowTypeVersion</span></span>|<span data-ttu-id="4ecc1-134">Одинарное</span><span class="sxs-lookup"><span data-stu-id="4ecc1-134">Single</span></span>| <span data-ttu-id="4ecc1-135">Это версия типа пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-135">This is the version of the user flow type.</span></span> <span data-ttu-id="4ecc1-136">Каждый тип пользовательского потока может иметь различные возможные версии, например 1, 1.1 или 2.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-136">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="4ecc1-137">Связи</span><span class="sxs-lookup"><span data-stu-id="4ecc1-137">Relationships</span></span>

<span data-ttu-id="4ecc1-138">Нет</span><span class="sxs-lookup"><span data-stu-id="4ecc1-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ecc1-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ecc1-139">JSON representation</span></span>

<span data-ttu-id="4ecc1-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ecc1-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "userFlowType": "string",
  "userFlowTypeVersion": "Single"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UserFlow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


