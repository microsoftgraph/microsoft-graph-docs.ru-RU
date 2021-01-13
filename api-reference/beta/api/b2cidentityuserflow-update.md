---
title: Обновление b2cIdentityUserFlow
description: Обновление свойств объекта b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f579b4772a9ee496b6f702d418d6b577bd4915db
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843663"
---
# <a name="update-b2cidentityuserflow"></a><span data-ttu-id="8d019-103">Обновление b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="8d019-103">Update b2cIdentityUserFlow</span></span>

<span data-ttu-id="8d019-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d019-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d019-105">Обновление свойств объекта [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="8d019-105">Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d019-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d019-106">Permissions</span></span>

<span data-ttu-id="8d019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d019-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d019-109">Permission type</span></span>      | <span data-ttu-id="8d019-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d019-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d019-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d019-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d019-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d019-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="8d019-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d019-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8d019-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d019-114">Not supported.</span></span>|
|<span data-ttu-id="8d019-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d019-115">Application</span></span>|<span data-ttu-id="8d019-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d019-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8d019-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="8d019-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8d019-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8d019-118">Global administrator</span></span>
* <span data-ttu-id="8d019-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="8d019-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8d019-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d019-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d019-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d019-121">Request headers</span></span>

|<span data-ttu-id="8d019-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8d019-122">Name</span></span>|<span data-ttu-id="8d019-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8d019-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8d019-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d019-124">Authorization</span></span>|<span data-ttu-id="8d019-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d019-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8d019-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d019-127">Content-Type</span></span>|<span data-ttu-id="8d019-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d019-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d019-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d019-130">Request body</span></span>

<span data-ttu-id="8d019-131">В теле запроса укажу представление объекта [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="8d019-131">In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

<span data-ttu-id="8d019-132">В следующей таблице показаны свойства, которые можно обновить после создания [объекта b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="8d019-132">The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="8d019-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d019-133">Property</span></span>|<span data-ttu-id="8d019-134">Тип</span><span class="sxs-lookup"><span data-stu-id="8d019-134">Type</span></span>|<span data-ttu-id="8d019-135">Описание</span><span class="sxs-lookup"><span data-stu-id="8d019-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d019-136">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="8d019-136">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="8d019-137">Логический</span><span class="sxs-lookup"><span data-stu-id="8d019-137">Boolean</span></span>|<span data-ttu-id="8d019-138">Свойство, определяющее, включена ли языковая настройка в пользовательском потоке B2C.</span><span class="sxs-lookup"><span data-stu-id="8d019-138">The property that determines whether language customization is enabled within the B2C user flow.</span></span> <span data-ttu-id="8d019-139">Настройка языка по умолчанию не включена для пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="8d019-139">Language customization is not enabled by default for B2C user flows.</span></span>|
|<span data-ttu-id="8d019-140">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="8d019-140">defaultLanguageTag</span></span>|<span data-ttu-id="8d019-141">Строка</span><span class="sxs-lookup"><span data-stu-id="8d019-141">String</span></span>|<span data-ttu-id="8d019-142">Указывает b2cIdentityUserFlow как язык по умолчанию, который используется, если в запросе не указан тег `ui_locale`.</span><span class="sxs-lookup"><span data-stu-id="8d019-142">Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="8d019-143">Это поле соответствует спецификации [RFC 5646](https://tools.ietf.org/html/rfc5646).</span><span class="sxs-lookup"><span data-stu-id="8d019-143">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|

## <a name="response"></a><span data-ttu-id="8d019-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d019-144">Response</span></span>

<span data-ttu-id="8d019-145">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d019-145">If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d019-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d019-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d019-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d019-147">Request</span></span>

<span data-ttu-id="8d019-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d019-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d019-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d019-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cidentityuserflow"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp
Content-Type: application/json
Content-length: 469

{
  "isLanguageCustomizationEnabled": true,
  "defaultLanguageTag": "en",
}
```
# <a name="javascript"></a>[<span data-ttu-id="8d019-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d019-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d019-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d019-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8d019-152">C#</span><span class="sxs-lookup"><span data-stu-id="8d019-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d019-153">Java</span><span class="sxs-lookup"><span data-stu-id="8d019-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d019-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d019-154">Response</span></span>

<span data-ttu-id="8d019-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d019-155">The following is an example of the response.</span></span>

<span data-ttu-id="8d019-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d019-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
}
-->

``` http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
