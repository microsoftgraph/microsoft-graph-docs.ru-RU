---
title: Тип ресурса UserFlow
description: Потоки пользователей удостоверений — это встроенные пути проверки подлинности
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a5cb0bfd61e9b99e9837c36484feefc0ff3a635
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440251"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="89fc8-103">Тип ресурса UserFlow</span><span class="sxs-lookup"><span data-stu-id="89fc8-103">UserFlow resource type</span></span>

<span data-ttu-id="89fc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89fc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89fc8-105">Потоки пользователей позволяют определять заранее настроенные политики для регистрации, регистрации, комбинированной регистрации и регистрации, сброса паролей и обновления профиля.</span><span class="sxs-lookup"><span data-stu-id="89fc8-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="89fc8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="89fc8-106">Methods</span></span>

| <span data-ttu-id="89fc8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="89fc8-107">Method</span></span>       | <span data-ttu-id="89fc8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89fc8-108">Return Type</span></span> | <span data-ttu-id="89fc8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89fc8-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="89fc8-110">Список</span><span class="sxs-lookup"><span data-stu-id="89fc8-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="89fc8-111">[Коллекция UserFlow](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="89fc8-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="89fc8-112">Список пользовательских процессов.</span><span class="sxs-lookup"><span data-stu-id="89fc8-112">List UserFlows.</span></span> |
| [<span data-ttu-id="89fc8-113">Создание</span><span class="sxs-lookup"><span data-stu-id="89fc8-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="89fc8-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="89fc8-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="89fc8-115">Создание объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="89fc8-115">Create UserFlow object.</span></span> |
| <span data-ttu-id="89fc8-116">[получение](../api/identityuserflow-get.md);</span><span class="sxs-lookup"><span data-stu-id="89fc8-116">[Get](../api/identityuserflow-get.md)</span></span> | [<span data-ttu-id="89fc8-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="89fc8-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="89fc8-118">Чтение свойств и связей объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="89fc8-118">Read properties and relationships of UserFlow object.</span></span> |
| <span data-ttu-id="89fc8-119">[удаление](../api/identityuserflow-delete.md);</span><span class="sxs-lookup"><span data-stu-id="89fc8-119">[Delete](../api/identityuserflow-delete.md)</span></span> | <span data-ttu-id="89fc8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="89fc8-120">None</span></span> | <span data-ttu-id="89fc8-121">Удаление объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="89fc8-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="89fc8-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="89fc8-122">Properties</span></span>

| <span data-ttu-id="89fc8-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="89fc8-123">Property</span></span>     | <span data-ttu-id="89fc8-124">Тип</span><span class="sxs-lookup"><span data-stu-id="89fc8-124">Type</span></span>        | <span data-ttu-id="89fc8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="89fc8-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="89fc8-126">id</span><span class="sxs-lookup"><span data-stu-id="89fc8-126">id</span></span>|<span data-ttu-id="89fc8-127">String</span><span class="sxs-lookup"><span data-stu-id="89fc8-127">String</span></span>| <span data-ttu-id="89fc8-128">Идентификатор потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="89fc8-128">The identifier of the user flow.</span></span> <span data-ttu-id="89fc8-129">Префикс **B2C_1_** добавляется к предоставляемой вами стоимости.</span><span class="sxs-lookup"><span data-stu-id="89fc8-129">The prefix of **B2C_1_** is added to the value that you provide.</span></span>|
|<span data-ttu-id="89fc8-130">userFlowType</span><span class="sxs-lookup"><span data-stu-id="89fc8-130">userFlowType</span></span>|<span data-ttu-id="89fc8-131">string</span><span class="sxs-lookup"><span data-stu-id="89fc8-131">string</span></span>| <span data-ttu-id="89fc8-132">Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="89fc8-132">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="89fc8-133">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="89fc8-133">userFlowTypeVersion</span></span>|<span data-ttu-id="89fc8-134">Одинарное</span><span class="sxs-lookup"><span data-stu-id="89fc8-134">Single</span></span>| <span data-ttu-id="89fc8-135">Это версия типа потока пользователя.</span><span class="sxs-lookup"><span data-stu-id="89fc8-135">This is the version of the user flow type.</span></span> <span data-ttu-id="89fc8-136">Каждый тип потока пользователей может иметь различные возможные версии, такие как 1, 1.1 или 2.</span><span class="sxs-lookup"><span data-stu-id="89fc8-136">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="89fc8-137">Связи</span><span class="sxs-lookup"><span data-stu-id="89fc8-137">Relationships</span></span>

<span data-ttu-id="89fc8-138">Нет</span><span class="sxs-lookup"><span data-stu-id="89fc8-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89fc8-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89fc8-139">JSON representation</span></span>

<span data-ttu-id="89fc8-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89fc8-140">The following is a JSON representation of the resource.</span></span>

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


