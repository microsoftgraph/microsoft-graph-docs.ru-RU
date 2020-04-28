---
title: Тип ресурса Усерфлов
description: Пользовательские потоки идентификации — это встроенные пути проверки подлинности
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d14722844c6449a585ca023df80fccb4e9d7c90b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218459"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="e268c-103">Тип ресурса Усерфлов</span><span class="sxs-lookup"><span data-stu-id="e268c-103">UserFlow resource type</span></span>

<span data-ttu-id="e268c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e268c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e268c-105">Потоки пользователей позволяют определить предопределенные настраиваемые политики для входа, регистрации, объединения и входа в систему, сброса пароля и обновления профиля.</span><span class="sxs-lookup"><span data-stu-id="e268c-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="e268c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e268c-106">Methods</span></span>

| <span data-ttu-id="e268c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e268c-107">Method</span></span>       | <span data-ttu-id="e268c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e268c-108">Return Type</span></span> | <span data-ttu-id="e268c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e268c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e268c-110">List</span><span class="sxs-lookup"><span data-stu-id="e268c-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="e268c-111">Коллекция [усерфлов](identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="e268c-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="e268c-112">Список Усерфловс.</span><span class="sxs-lookup"><span data-stu-id="e268c-112">List UserFlows.</span></span> |
| <span data-ttu-id="e268c-113">[создание](../api/identityuserflow-post-userflows.md);</span><span class="sxs-lookup"><span data-stu-id="e268c-113">[Create](../api/identityuserflow-post-userflows.md)</span></span> | [<span data-ttu-id="e268c-114">усерфлов</span><span class="sxs-lookup"><span data-stu-id="e268c-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="e268c-115">Создание объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="e268c-115">Create UserFlow object.</span></span> |
| <span data-ttu-id="e268c-116">[получение](../api/identityuserflow-get.md);</span><span class="sxs-lookup"><span data-stu-id="e268c-116">[Get](../api/identityuserflow-get.md)</span></span> | [<span data-ttu-id="e268c-117">усерфлов</span><span class="sxs-lookup"><span data-stu-id="e268c-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="e268c-118">Чтение свойств и связей объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="e268c-118">Read properties and relationships of UserFlow object.</span></span> |
| <span data-ttu-id="e268c-119">[удаление](../api/identityuserflow-delete.md);</span><span class="sxs-lookup"><span data-stu-id="e268c-119">[Delete](../api/identityuserflow-delete.md)</span></span> | <span data-ttu-id="e268c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e268c-120">None</span></span> | <span data-ttu-id="e268c-121">Удаление объекта Усерфлов.</span><span class="sxs-lookup"><span data-stu-id="e268c-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e268c-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="e268c-122">Properties</span></span>

| <span data-ttu-id="e268c-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="e268c-123">Property</span></span>     | <span data-ttu-id="e268c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e268c-124">Type</span></span>        | <span data-ttu-id="e268c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e268c-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e268c-126">id</span><span class="sxs-lookup"><span data-stu-id="e268c-126">id</span></span>|<span data-ttu-id="e268c-127">String</span><span class="sxs-lookup"><span data-stu-id="e268c-127">String</span></span>| <span data-ttu-id="e268c-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e268c-128">Read-only.</span></span>|
|<span data-ttu-id="e268c-129">усерфловтипе</span><span class="sxs-lookup"><span data-stu-id="e268c-129">userFlowType</span></span>|<span data-ttu-id="e268c-130">string</span><span class="sxs-lookup"><span data-stu-id="e268c-130">string</span></span>| <span data-ttu-id="e268c-131">Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e268c-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e268c-132">усерфловтипеверсион</span><span class="sxs-lookup"><span data-stu-id="e268c-132">userFlowTypeVersion</span></span>|<span data-ttu-id="e268c-133">Одинарное</span><span class="sxs-lookup"><span data-stu-id="e268c-133">Single</span></span>| <span data-ttu-id="e268c-134">Это версия пользовательского типа.</span><span class="sxs-lookup"><span data-stu-id="e268c-134">This is the version of the user flow type.</span></span> <span data-ttu-id="e268c-135">Каждый тип пользовательского типа может иметь различные варианты, например 1, 1,1 или 2.</span><span class="sxs-lookup"><span data-stu-id="e268c-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="e268c-136">Связи</span><span class="sxs-lookup"><span data-stu-id="e268c-136">Relationships</span></span>

<span data-ttu-id="e268c-137">Нет</span><span class="sxs-lookup"><span data-stu-id="e268c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e268c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e268c-138">JSON representation</span></span>

<span data-ttu-id="e268c-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e268c-139">The following is a JSON representation of the resource.</span></span>

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
