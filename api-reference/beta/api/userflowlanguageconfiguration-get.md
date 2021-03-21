---
title: Get userFlowLanguageConfiguration
description: Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 25fa30b9904854ce027c503cf738cabd55ce5567
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955262"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="816a0-103">Get userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="816a0-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="816a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="816a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="816a0-105">Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="816a0-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="816a0-106">Эти объекты представляют язык, доступный в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="816a0-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="816a0-107">**Примечание:** Чтобы получить язык, поддерживаемый для настройки, сначала необходимо включить настройку языка в потоке пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="816a0-107">**Note:** To retrieve a language supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="816a0-108">Дополнительные сведения см. [в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="816a0-108">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span> <span data-ttu-id="816a0-109">Настройка языка включена по умолчанию в [потоках пользователей Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="816a0-109">Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="816a0-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="816a0-110">Permissions</span></span>

<span data-ttu-id="816a0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="816a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="816a0-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="816a0-113">Permission type</span></span>      | <span data-ttu-id="816a0-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="816a0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="816a0-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="816a0-115">Delegated (work or school account)</span></span>|<span data-ttu-id="816a0-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="816a0-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="816a0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="816a0-117">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="816a0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="816a0-118">Not supported.</span></span>|
|<span data-ttu-id="816a0-119">Application</span><span class="sxs-lookup"><span data-stu-id="816a0-119">Application</span></span>|<span data-ttu-id="816a0-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="816a0-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="816a0-121">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="816a0-121">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="816a0-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="816a0-122">Global administrator</span></span>
* <span data-ttu-id="816a0-123">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="816a0-123">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="816a0-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="816a0-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/languages/{id}
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="816a0-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="816a0-125">Request headers</span></span>

|<span data-ttu-id="816a0-126">Имя</span><span class="sxs-lookup"><span data-stu-id="816a0-126">Name</span></span>|<span data-ttu-id="816a0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="816a0-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="816a0-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="816a0-128">Authorization</span></span>|<span data-ttu-id="816a0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="816a0-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="816a0-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="816a0-131">Request body</span></span>

<span data-ttu-id="816a0-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="816a0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="816a0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="816a0-133">Response</span></span>

<span data-ttu-id="816a0-134">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="816a0-134">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="816a0-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="816a0-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="816a0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="816a0-136">Request</span></span>

<span data-ttu-id="816a0-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="816a0-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="816a0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="816a0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en
```
# <a name="c"></a>[<span data-ttu-id="816a0-139">C#</span><span class="sxs-lookup"><span data-stu-id="816a0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="816a0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="816a0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="816a0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="816a0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="816a0-142">Java</span><span class="sxs-lookup"><span data-stu-id="816a0-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="816a0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="816a0-143">Response</span></span>

<span data-ttu-id="816a0-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="816a0-144">The following is an example of the response.</span></span>

<span data-ttu-id="816a0-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="816a0-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_Customer')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
