---
title: Тип ресурса UserFlow
description: Представляет поток пользователей удостоверений, включенный во встроенное путешествие по проверке подлинности.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4e03faaff265bf82bacf16a2db6c75e81176eafa
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883007"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="6f265-103">Тип ресурса UserFlow</span><span class="sxs-lookup"><span data-stu-id="6f265-103">UserFlow resource type</span></span>

<span data-ttu-id="6f265-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f265-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f265-105">Потоки пользователей позволяют определить заранее настроенные политики для регистрации, регистрации, комбинированной регистрации и регистрации, сброса пароля и обновления профиля.</span><span class="sxs-lookup"><span data-stu-id="6f265-105">User Flows enable you to define predefined, configurable policies for sign-in, sign-up, combined sign-up and sign-in, password reset, and profile update.</span></span> <span data-ttu-id="6f265-106">Это базовый класс, который наследуют другие потоки пользователей.</span><span class="sxs-lookup"><span data-stu-id="6f265-106">This is a base class that other user flows inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="6f265-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f265-107">Properties</span></span>

| <span data-ttu-id="6f265-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f265-108">Property</span></span>     | <span data-ttu-id="6f265-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6f265-109">Type</span></span>        | <span data-ttu-id="6f265-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f265-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f265-111">id</span><span class="sxs-lookup"><span data-stu-id="6f265-111">id</span></span>|<span data-ttu-id="6f265-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6f265-112">String</span></span>| <span data-ttu-id="6f265-113">Идентификатор потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6f265-113">The identifier of the user flow.</span></span> <span data-ttu-id="6f265-114">Префикс **B2C_1_** добавляется к предоставляемой вами стоимости.</span><span class="sxs-lookup"><span data-stu-id="6f265-114">The prefix of **B2C_1_** is added to the value that you provide.</span></span>|
|<span data-ttu-id="6f265-115">userFlowType</span><span class="sxs-lookup"><span data-stu-id="6f265-115">userFlowType</span></span>|<span data-ttu-id="6f265-116">userFlowType</span><span class="sxs-lookup"><span data-stu-id="6f265-116">userFlowType</span></span>| <span data-ttu-id="6f265-117">Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6f265-117">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6f265-118">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="6f265-118">userFlowTypeVersion</span></span>|<span data-ttu-id="6f265-119">Одинарное</span><span class="sxs-lookup"><span data-stu-id="6f265-119">Single</span></span>| <span data-ttu-id="6f265-120">Это версия типа потока пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f265-120">This is the version of the user flow type.</span></span> <span data-ttu-id="6f265-121">Каждый тип потока пользователей может иметь различные возможные версии, такие как 1, 1.1 или 2.</span><span class="sxs-lookup"><span data-stu-id="6f265-121">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="6f265-122">Связи</span><span class="sxs-lookup"><span data-stu-id="6f265-122">Relationships</span></span>

<span data-ttu-id="6f265-123">Нет</span><span class="sxs-lookup"><span data-stu-id="6f265-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f265-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f265-124">JSON representation</span></span>

<span data-ttu-id="6f265-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f265-125">The following is a JSON representation of the resource.</span></span>

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
