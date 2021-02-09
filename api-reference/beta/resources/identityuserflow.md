---
title: Тип ресурса UserFlow
description: Потоки пользователей удостоверений — это встроенные пути проверки подлинности
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b4842b506e3c3c3e675ec2a47837fbf0c2e10be
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158291"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="fcb63-103">Тип ресурса UserFlow</span><span class="sxs-lookup"><span data-stu-id="fcb63-103">UserFlow resource type</span></span>

<span data-ttu-id="fcb63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcb63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcb63-105">Потоки пользователей позволяют определять предварительно определенные настраиваемые политики для входов, регистрации, объединенной регистрации и входов, сброса паролей и обновления профиля.</span><span class="sxs-lookup"><span data-stu-id="fcb63-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="fcb63-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fcb63-106">Methods</span></span>

| <span data-ttu-id="fcb63-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fcb63-107">Method</span></span>       | <span data-ttu-id="fcb63-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fcb63-108">Return Type</span></span> | <span data-ttu-id="fcb63-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fcb63-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fcb63-110">Список</span><span class="sxs-lookup"><span data-stu-id="fcb63-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="fcb63-111">[Коллекция UserFlow](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="fcb63-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="fcb63-112">Список userFlows.</span><span class="sxs-lookup"><span data-stu-id="fcb63-112">List UserFlows.</span></span> |
| [<span data-ttu-id="fcb63-113">Создание</span><span class="sxs-lookup"><span data-stu-id="fcb63-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="fcb63-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="fcb63-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="fcb63-115">Создание объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="fcb63-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="fcb63-116">Получение</span><span class="sxs-lookup"><span data-stu-id="fcb63-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="fcb63-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="fcb63-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="fcb63-118">Чтение свойств и связей объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="fcb63-118">Read properties and relationships of UserFlow object.</span></span> |
| <span data-ttu-id="fcb63-119">[удаление](../api/identityuserflow-delete.md);</span><span class="sxs-lookup"><span data-stu-id="fcb63-119">[Delete](../api/identityuserflow-delete.md)</span></span> | <span data-ttu-id="fcb63-120">Нет</span><span class="sxs-lookup"><span data-stu-id="fcb63-120">None</span></span> | <span data-ttu-id="fcb63-121">Удаление объекта UserFlow.</span><span class="sxs-lookup"><span data-stu-id="fcb63-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fcb63-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcb63-122">Properties</span></span>

| <span data-ttu-id="fcb63-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcb63-123">Property</span></span>     | <span data-ttu-id="fcb63-124">Тип</span><span class="sxs-lookup"><span data-stu-id="fcb63-124">Type</span></span>        | <span data-ttu-id="fcb63-125">Описание</span><span class="sxs-lookup"><span data-stu-id="fcb63-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fcb63-126">id</span><span class="sxs-lookup"><span data-stu-id="fcb63-126">id</span></span>|<span data-ttu-id="fcb63-127">String</span><span class="sxs-lookup"><span data-stu-id="fcb63-127">String</span></span>| <span data-ttu-id="fcb63-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcb63-128">Read-only.</span></span>|
|<span data-ttu-id="fcb63-129">userFlowType</span><span class="sxs-lookup"><span data-stu-id="fcb63-129">userFlowType</span></span>|<span data-ttu-id="fcb63-130">string</span><span class="sxs-lookup"><span data-stu-id="fcb63-130">string</span></span>| <span data-ttu-id="fcb63-131">Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fcb63-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fcb63-132">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="fcb63-132">userFlowTypeVersion</span></span>|<span data-ttu-id="fcb63-133">Одинарное</span><span class="sxs-lookup"><span data-stu-id="fcb63-133">Single</span></span>| <span data-ttu-id="fcb63-134">Это версия типа пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="fcb63-134">This is the version of the user flow type.</span></span> <span data-ttu-id="fcb63-135">Каждый тип пользовательского потока может иметь различные возможные версии, например 1, 1.1 или 2.</span><span class="sxs-lookup"><span data-stu-id="fcb63-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="fcb63-136">Связи</span><span class="sxs-lookup"><span data-stu-id="fcb63-136">Relationships</span></span>

<span data-ttu-id="fcb63-137">Нет</span><span class="sxs-lookup"><span data-stu-id="fcb63-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcb63-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcb63-138">JSON representation</span></span>

<span data-ttu-id="fcb63-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcb63-139">The following is a JSON representation of the resource.</span></span>

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


