---
title: Тип ресурса Усерфлов
description: Пользовательские потоки идентификации — это встроенные пути проверки подлинности
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4fa3064d19d96a2a8297f72de6a625ee36c8db3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496553"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="7405e-103">Тип ресурса Усерфлов</span><span class="sxs-lookup"><span data-stu-id="7405e-103">UserFlow resource type</span></span>

<span data-ttu-id="7405e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7405e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7405e-105">Потоки пользователей позволяют определить предопределенные настраиваемые политики для входа, регистрации, объединения и входа в систему, сброса пароля и обновления профиля.</span><span class="sxs-lookup"><span data-stu-id="7405e-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="7405e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7405e-106">Methods</span></span>

| <span data-ttu-id="7405e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7405e-107">Method</span></span>       | <span data-ttu-id="7405e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7405e-108">Return Type</span></span> | <span data-ttu-id="7405e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7405e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7405e-110">List</span><span class="sxs-lookup"><span data-stu-id="7405e-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="7405e-111">Коллекция [усерфлов](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="7405e-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="7405e-112">Список Усерфловс.</span><span class="sxs-lookup"><span data-stu-id="7405e-112">List UserFlows.</span></span> |
| <span data-ttu-id="7405e-113">[создание](../api/identityuserflow-post-userflows.md);</span><span class="sxs-lookup"><span data-stu-id="7405e-113">[Create](../api/identityuserflow-post-userflows.md)</span></span> | [<span data-ttu-id="7405e-114">усерфлов</span><span class="sxs-lookup"><span data-stu-id="7405e-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="7405e-115">Создание объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="7405e-115">Create UserFlow object.</span></span> |
| <span data-ttu-id="7405e-116">[получение](../api/identityuserflow-get.md);</span><span class="sxs-lookup"><span data-stu-id="7405e-116">[Get](../api/identityuserflow-get.md)</span></span> | [<span data-ttu-id="7405e-117">усерфлов</span><span class="sxs-lookup"><span data-stu-id="7405e-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="7405e-118">Чтение свойств и связей объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="7405e-118">Read properties and relationships of UserFlow object.</span></span> |
| <span data-ttu-id="7405e-119">[удаление](../api/identityuserflow-delete.md);</span><span class="sxs-lookup"><span data-stu-id="7405e-119">[Delete](../api/identityuserflow-delete.md)</span></span> | <span data-ttu-id="7405e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7405e-120">None</span></span> | <span data-ttu-id="7405e-121">Удаление объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="7405e-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7405e-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="7405e-122">Properties</span></span>

| <span data-ttu-id="7405e-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="7405e-123">Property</span></span>     | <span data-ttu-id="7405e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7405e-124">Type</span></span>        | <span data-ttu-id="7405e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7405e-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7405e-126">id</span><span class="sxs-lookup"><span data-stu-id="7405e-126">id</span></span>|<span data-ttu-id="7405e-127">String</span><span class="sxs-lookup"><span data-stu-id="7405e-127">String</span></span>| <span data-ttu-id="7405e-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7405e-128">Read-only.</span></span>|
|<span data-ttu-id="7405e-129">усерфловтипе</span><span class="sxs-lookup"><span data-stu-id="7405e-129">userFlowType</span></span>|<span data-ttu-id="7405e-130">строка</span><span class="sxs-lookup"><span data-stu-id="7405e-130">string</span></span>| <span data-ttu-id="7405e-131">Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7405e-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7405e-132">усерфловтипеверсион</span><span class="sxs-lookup"><span data-stu-id="7405e-132">userFlowTypeVersion</span></span>|<span data-ttu-id="7405e-133">Одинарное</span><span class="sxs-lookup"><span data-stu-id="7405e-133">Single</span></span>| <span data-ttu-id="7405e-134">Это версия пользовательского типа.</span><span class="sxs-lookup"><span data-stu-id="7405e-134">This is the version of the user flow type.</span></span> <span data-ttu-id="7405e-135">Каждый тип пользовательского типа может иметь различные варианты, например 1, 1,1 или 2.</span><span class="sxs-lookup"><span data-stu-id="7405e-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="7405e-136">Связи</span><span class="sxs-lookup"><span data-stu-id="7405e-136">Relationships</span></span>

<span data-ttu-id="7405e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="7405e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7405e-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7405e-138">JSON representation</span></span>

<span data-ttu-id="7405e-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7405e-139">The following is a JSON representation of the resource.</span></span>

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
