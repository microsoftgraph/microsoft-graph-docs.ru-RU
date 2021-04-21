---
title: Get userFlowLanguageConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта userFlowLanguageConfiguration.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a2f17c309e104738a1bae4fd7e599fd8efa28355
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920585"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="ba759-103">Get userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba759-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="ba759-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba759-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba759-105">Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba759-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="ba759-106">Эти объекты представляют язык, доступный в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="ba759-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="ba759-107">**Примечание:** Настройка языка включена по умолчанию в [потоках пользователей Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="ba759-107">**Note:** Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba759-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba759-108">Permissions</span></span>

<span data-ttu-id="ba759-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba759-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba759-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba759-111">Permission type</span></span>      | <span data-ttu-id="ba759-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba759-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba759-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba759-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba759-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba759-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ba759-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba759-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ba759-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba759-116">Not supported.</span></span>|
|<span data-ttu-id="ba759-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba759-117">Application</span></span>|<span data-ttu-id="ba759-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba759-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ba759-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ba759-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ba759-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ba759-120">Global administrator</span></span>
* <span data-ttu-id="ba759-121">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="ba759-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ba759-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba759-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba759-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba759-123">Request headers</span></span>

|<span data-ttu-id="ba759-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ba759-124">Name</span></span>|<span data-ttu-id="ba759-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ba759-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba759-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba759-126">Authorization</span></span>|<span data-ttu-id="ba759-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba759-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba759-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba759-129">Request body</span></span>

<span data-ttu-id="ba759-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba759-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba759-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba759-131">Response</span></span>

<span data-ttu-id="ba759-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ba759-132">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba759-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba759-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba759-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba759-134">Request</span></span>

<span data-ttu-id="ba759-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba759-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba759-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba759-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en
```
# <a name="c"></a>[<span data-ttu-id="ba759-137">C#</span><span class="sxs-lookup"><span data-stu-id="ba759-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba759-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba759-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba759-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba759-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba759-140">Java</span><span class="sxs-lookup"><span data-stu-id="ba759-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba759-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba759-141">Response</span></span>

<span data-ttu-id="ba759-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba759-142">The following is an example of the response.</span></span>

<span data-ttu-id="ba759-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ba759-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_Partner')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
