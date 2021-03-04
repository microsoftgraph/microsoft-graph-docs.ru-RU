---
title: тип ресурса emailAuthenticationMethod
description: Представление адреса электронной почты, зарегистрированного пользователем. Электронная почта — это метод проверки подлинности, доступный только для сброса пароля самообслуживления (SSPR)
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a24a67fdb4bcc054036de26ba235bf4bac0f2da2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440369"
---
# <a name="emailauthenticationmethod-resource-type"></a><span data-ttu-id="c34b0-104">тип ресурса emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c34b0-104">emailAuthenticationMethod resource type</span></span>

<span data-ttu-id="c34b0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c34b0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c34b0-106">Представление адреса электронной почты, зарегистрированного пользователем.</span><span class="sxs-lookup"><span data-stu-id="c34b0-106">A representation of an email address registered to a user.</span></span> <span data-ttu-id="c34b0-107">Электронная почта — это метод проверки подлинности, доступный только для сброса пароля самообслуживления (SSPR).</span><span class="sxs-lookup"><span data-stu-id="c34b0-107">Email is an authentication method available only to self-service password reset (SSPR).</span></span> <span data-ttu-id="c34b0-108">У пользователей может быть только один метод проверки подлинности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c34b0-108">Users may only have one email authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="c34b0-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c34b0-109">Methods</span></span>
|<span data-ttu-id="c34b0-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c34b0-110">Method</span></span>|<span data-ttu-id="c34b0-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="c34b0-111">Return type</span></span>|<span data-ttu-id="c34b0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c34b0-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c34b0-113">Список</span><span class="sxs-lookup"><span data-stu-id="c34b0-113">List</span></span>](../api/emailauthenticationmethod-list.md)|<span data-ttu-id="c34b0-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection</span><span class="sxs-lookup"><span data-stu-id="c34b0-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection</span></span>|<span data-ttu-id="c34b0-115">Извлечение списка электронной почты пользователяAuthenticationMethods.</span><span class="sxs-lookup"><span data-stu-id="c34b0-115">Retrieve a list of a user's emailAuthenticationMethods.</span></span> <span data-ttu-id="c34b0-116">У пользователей может быть только один метод проверки подлинности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c34b0-116">Users may only have one email authentication method.</span></span>|
|[<span data-ttu-id="c34b0-117">Создание</span><span class="sxs-lookup"><span data-stu-id="c34b0-117">Create</span></span>](../api/emailauthenticationmethod-post.md)|[<span data-ttu-id="c34b0-118">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c34b0-118">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="c34b0-119">Создайте объект электронной почты пользователяMethods.</span><span class="sxs-lookup"><span data-stu-id="c34b0-119">Create a user's emailMethods object.</span></span>|
|<span data-ttu-id="c34b0-120">[получение](../api/emailauthenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="c34b0-120">[Get](../api/emailauthenticationmethod-get.md)</span></span>|[<span data-ttu-id="c34b0-121">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c34b0-121">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="c34b0-122">Извлечение свойств объекта электронной почты пользователяAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="c34b0-122">Retrieve the properties  of the user's emailAuthenticationMethod object.</span></span>|
|[<span data-ttu-id="c34b0-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="c34b0-123">Update</span></span>](../api/emailauthenticationmethod-update.md)|[<span data-ttu-id="c34b0-124">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c34b0-124">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="c34b0-125">Обновление свойств объекта электронной почты пользователяMethods.</span><span class="sxs-lookup"><span data-stu-id="c34b0-125">Update the properties of a user's emailMethods object.</span></span>|
|<span data-ttu-id="c34b0-126">[удаление](../api/emailauthenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="c34b0-126">[Delete](../api/emailauthenticationmethod-delete.md)</span></span>|<span data-ttu-id="c34b0-127">Нет</span><span class="sxs-lookup"><span data-stu-id="c34b0-127">None</span></span>|<span data-ttu-id="c34b0-128">Удаление объекта электронной почты пользователяAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="c34b0-128">Delete a user's emailAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="c34b0-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="c34b0-129">Properties</span></span>
|<span data-ttu-id="c34b0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c34b0-130">Property</span></span>|<span data-ttu-id="c34b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c34b0-131">Type</span></span>|<span data-ttu-id="c34b0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c34b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c34b0-133">id</span><span class="sxs-lookup"><span data-stu-id="c34b0-133">id</span></span>|<span data-ttu-id="c34b0-134">String</span><span class="sxs-lookup"><span data-stu-id="c34b0-134">String</span></span>|<span data-ttu-id="c34b0-135">Идентификатор адреса электронной почты, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c34b0-135">The identifier of the email address registered to this user.</span></span>|
|<span data-ttu-id="c34b0-136">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c34b0-136">emailAddress</span></span>|<span data-ttu-id="c34b0-137">String</span><span class="sxs-lookup"><span data-stu-id="c34b0-137">String</span></span>|<span data-ttu-id="c34b0-138">Адрес электронной почты, зарегистрированный для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c34b0-138">The email address registered to this user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c34b0-139">Связи</span><span class="sxs-lookup"><span data-stu-id="c34b0-139">Relationships</span></span>
<span data-ttu-id="c34b0-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c34b0-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c34b0-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c34b0-141">JSON representation</span></span>
<span data-ttu-id="c34b0-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c34b0-142">The following is a JSON representation of the resource.</span></span>
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

