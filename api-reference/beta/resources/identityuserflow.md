---
title: Тип ресурса Усерфлов
description: Пользовательские потоки идентификации — это встроенные пути проверки подлинности
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5410b65dfdb0841aa997022b43dc04d0a4627008
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734676"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="437a3-103">Тип ресурса Усерфлов</span><span class="sxs-lookup"><span data-stu-id="437a3-103">UserFlow resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="437a3-104">Потоки пользователей позволяют определить предопределенные настраиваемые политики для входа, регистрации, объединения и входа в систему, сброса пароля и обновления профиля.</span><span class="sxs-lookup"><span data-stu-id="437a3-104">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="437a3-105">Методы</span><span class="sxs-lookup"><span data-stu-id="437a3-105">Methods</span></span>

| <span data-ttu-id="437a3-106">Метод</span><span class="sxs-lookup"><span data-stu-id="437a3-106">Method</span></span>       | <span data-ttu-id="437a3-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="437a3-107">Return Type</span></span> | <span data-ttu-id="437a3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="437a3-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="437a3-109">List</span><span class="sxs-lookup"><span data-stu-id="437a3-109">List</span></span>](../api/identityuserflow-list.md) | [<span data-ttu-id="437a3-110">усерфлов</span><span class="sxs-lookup"><span data-stu-id="437a3-110">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="437a3-111">Список Усерфловс.</span><span class="sxs-lookup"><span data-stu-id="437a3-111">List UserFlows.</span></span> |
| <span data-ttu-id="437a3-112">[создание](../api/identityuserflow-post-userflows.md);</span><span class="sxs-lookup"><span data-stu-id="437a3-112">[Create](../api/identityuserflow-post-userflows.md)</span></span> | <span data-ttu-id="437a3-113">Нет</span><span class="sxs-lookup"><span data-stu-id="437a3-113">None</span></span> | <span data-ttu-id="437a3-114">Создание объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="437a3-114">Create UserFlow object.</span></span> |
| <span data-ttu-id="437a3-115">[получение](../api/identityuserflow-get.md);</span><span class="sxs-lookup"><span data-stu-id="437a3-115">[Get](../api/identityuserflow-get.md)</span></span> | [<span data-ttu-id="437a3-116">усерфлов</span><span class="sxs-lookup"><span data-stu-id="437a3-116">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="437a3-117">Чтение свойств и связей объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="437a3-117">Read properties and relationships of UserFlow object.</span></span> |
| <span data-ttu-id="437a3-118">[удаление](../api/identityuserflow-delete.md);</span><span class="sxs-lookup"><span data-stu-id="437a3-118">[Delete](../api/identityuserflow-delete.md)</span></span> | <span data-ttu-id="437a3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="437a3-119">None</span></span> | <span data-ttu-id="437a3-120">Удаление объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="437a3-120">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="437a3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="437a3-121">Properties</span></span>

| <span data-ttu-id="437a3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="437a3-122">Property</span></span>     | <span data-ttu-id="437a3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="437a3-123">Type</span></span>        | <span data-ttu-id="437a3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="437a3-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="437a3-125">id</span><span class="sxs-lookup"><span data-stu-id="437a3-125">id</span></span>|<span data-ttu-id="437a3-126">String</span><span class="sxs-lookup"><span data-stu-id="437a3-126">String</span></span>| <span data-ttu-id="437a3-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="437a3-127">Read-only.</span></span>|
|<span data-ttu-id="437a3-128">усерфловтипе</span><span class="sxs-lookup"><span data-stu-id="437a3-128">userFlowType</span></span>|<span data-ttu-id="437a3-129">string</span><span class="sxs-lookup"><span data-stu-id="437a3-129">string</span></span>| <span data-ttu-id="437a3-130">Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="437a3-130">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="437a3-131">усерфловтипеверсион</span><span class="sxs-lookup"><span data-stu-id="437a3-131">userFlowTypeVersion</span></span>|<span data-ttu-id="437a3-132">Одинарное</span><span class="sxs-lookup"><span data-stu-id="437a3-132">Single</span></span>| <span data-ttu-id="437a3-133">Это версия пользовательского типа.</span><span class="sxs-lookup"><span data-stu-id="437a3-133">This is the version of the user flow type.</span></span> <span data-ttu-id="437a3-134">Каждый тип пользовательского типа может иметь различные варианты, например 1, 1,1 или 2.</span><span class="sxs-lookup"><span data-stu-id="437a3-134">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="437a3-135">Связи</span><span class="sxs-lookup"><span data-stu-id="437a3-135">Relationships</span></span>

<span data-ttu-id="437a3-136">Нет</span><span class="sxs-lookup"><span data-stu-id="437a3-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="437a3-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="437a3-137">JSON representation</span></span>

<span data-ttu-id="437a3-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="437a3-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "baseType": "",
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
