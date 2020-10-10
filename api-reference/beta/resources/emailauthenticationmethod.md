---
title: Тип ресурса Емаилаусентикатионмесод
description: Представление адреса электронной почты, зарегистрированного для пользователя. Электронная почта — способ проверки подлинности, доступный только для самостоятельного сброса пароля (SSPR)
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6dde3c9a859f2527241b66c0172d6b5dd877aac4
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418475"
---
# <a name="emailauthenticationmethod-resource-type"></a><span data-ttu-id="0d19d-104">Тип ресурса Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0d19d-104">emailAuthenticationMethod resource type</span></span>

<span data-ttu-id="0d19d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d19d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d19d-106">Представление адреса электронной почты, зарегистрированного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d19d-106">A representation of an email address registered to a user.</span></span> <span data-ttu-id="0d19d-107">Электронная почта — это способ проверки подлинности, доступный только для самостоятельного сброса пароля (SSPR).</span><span class="sxs-lookup"><span data-stu-id="0d19d-107">Email is an authentication method available only to self-service password reset (SSPR).</span></span> <span data-ttu-id="0d19d-108">У пользователей может быть только один способ проверки подлинности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0d19d-108">Users may only have one email authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="0d19d-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0d19d-109">Methods</span></span>
|<span data-ttu-id="0d19d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0d19d-110">Method</span></span>|<span data-ttu-id="0d19d-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="0d19d-111">Return type</span></span>|<span data-ttu-id="0d19d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0d19d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0d19d-113">Перечисление</span><span class="sxs-lookup"><span data-stu-id="0d19d-113">List</span></span>](../api/emailauthenticationmethod-list.md)|<span data-ttu-id="0d19d-114">Коллекция [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="0d19d-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection</span></span>|<span data-ttu-id="0d19d-115">Получение списка Емаилаусентикатионмесодс пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d19d-115">Retrieve a list of a user's emailAuthenticationMethods.</span></span> <span data-ttu-id="0d19d-116">У пользователей может быть только один способ проверки подлинности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0d19d-116">Users may only have one email authentication method.</span></span>|
|[<span data-ttu-id="0d19d-117">Создание</span><span class="sxs-lookup"><span data-stu-id="0d19d-117">Create</span></span>](../api/emailauthenticationmethod-post.md)|[<span data-ttu-id="0d19d-118">емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0d19d-118">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="0d19d-119">Создание объекта Емаилмесодс пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d19d-119">Create a user's emailMethods object.</span></span>|
|[<span data-ttu-id="0d19d-120">Получение</span><span class="sxs-lookup"><span data-stu-id="0d19d-120">Get</span></span>](../api/emailauthenticationmethod-get.md)|[<span data-ttu-id="0d19d-121">емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0d19d-121">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="0d19d-122">Получение свойств объекта Емаилаусентикатионмесод пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d19d-122">Retrieve the properties  of the user's emailAuthenticationMethod object.</span></span>|
|[<span data-ttu-id="0d19d-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="0d19d-123">Update</span></span>](../api/emailauthenticationmethod-update.md)|[<span data-ttu-id="0d19d-124">емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0d19d-124">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="0d19d-125">Обновление свойств объекта Емаилмесодс пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d19d-125">Update the properties of a user's emailMethods object.</span></span>|
|[<span data-ttu-id="0d19d-126">Удаление</span><span class="sxs-lookup"><span data-stu-id="0d19d-126">Delete</span></span>](../api/emailauthenticationmethod-delete.md)|<span data-ttu-id="0d19d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0d19d-127">None</span></span>|<span data-ttu-id="0d19d-128">Удаление объекта Емаилаусентикатионмесод пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d19d-128">Delete a user's emailAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="0d19d-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d19d-129">Properties</span></span>
|<span data-ttu-id="0d19d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d19d-130">Property</span></span>|<span data-ttu-id="0d19d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0d19d-131">Type</span></span>|<span data-ttu-id="0d19d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0d19d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d19d-133">id</span><span class="sxs-lookup"><span data-stu-id="0d19d-133">id</span></span>|<span data-ttu-id="0d19d-134">String</span><span class="sxs-lookup"><span data-stu-id="0d19d-134">String</span></span>|<span data-ttu-id="0d19d-135">Идентификатор адреса электронной почты, зарегистрированный для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d19d-135">The identifier of the email address registered to this user.</span></span>|
|<span data-ttu-id="0d19d-136">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0d19d-136">emailAddress</span></span>|<span data-ttu-id="0d19d-137">String</span><span class="sxs-lookup"><span data-stu-id="0d19d-137">String</span></span>|<span data-ttu-id="0d19d-138">Адрес электронной почты, зарегистрированный для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d19d-138">The email address registered to this user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d19d-139">Связи</span><span class="sxs-lookup"><span data-stu-id="0d19d-139">Relationships</span></span>
<span data-ttu-id="0d19d-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0d19d-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d19d-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0d19d-141">JSON representation</span></span>
<span data-ttu-id="0d19d-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d19d-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethod",
  "id": "String (identifier)",
  "emailAddress": "String"
}
```

