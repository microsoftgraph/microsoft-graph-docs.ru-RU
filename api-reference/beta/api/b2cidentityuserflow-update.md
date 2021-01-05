---
title: Обновление b2cIdentityUserFlow
description: Обновление свойств объекта b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fb11cd2f9dc547499091876e1bdf6130819d270
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753133"
---
# <a name="update-b2cidentityuserflow"></a><span data-ttu-id="cb2ec-103">Обновление b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="cb2ec-103">Update b2cIdentityUserFlow</span></span>

<span data-ttu-id="cb2ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb2ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb2ec-105">Обновление свойств объекта [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="cb2ec-105">Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb2ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb2ec-106">Permissions</span></span>

<span data-ttu-id="cb2ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb2ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb2ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb2ec-109">Permission type</span></span>      | <span data-ttu-id="cb2ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb2ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb2ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb2ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb2ec-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb2ec-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="cb2ec-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb2ec-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="cb2ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-114">Not supported.</span></span>|
|<span data-ttu-id="cb2ec-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb2ec-115">Application</span></span>|<span data-ttu-id="cb2ec-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb2ec-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="cb2ec-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="cb2ec-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="cb2ec-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="cb2ec-118">Global administrator</span></span>
* <span data-ttu-id="cb2ec-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="cb2ec-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="cb2ec-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb2ec-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cb2ec-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb2ec-121">Request headers</span></span>

|<span data-ttu-id="cb2ec-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cb2ec-122">Name</span></span>|<span data-ttu-id="cb2ec-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cb2ec-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb2ec-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb2ec-124">Authorization</span></span>|<span data-ttu-id="cb2ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cb2ec-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb2ec-127">Content-Type</span></span>|<span data-ttu-id="cb2ec-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb2ec-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb2ec-130">Request body</span></span>

<span data-ttu-id="cb2ec-131">В теле запроса укажу представление объекта [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-131">In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

<span data-ttu-id="cb2ec-132">В следующей таблице показаны свойства, которые можно обновить после создания [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="cb2ec-132">The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="cb2ec-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb2ec-133">Property</span></span>|<span data-ttu-id="cb2ec-134">Тип</span><span class="sxs-lookup"><span data-stu-id="cb2ec-134">Type</span></span>|<span data-ttu-id="cb2ec-135">Описание</span><span class="sxs-lookup"><span data-stu-id="cb2ec-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb2ec-136">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="cb2ec-136">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="cb2ec-137">Логический</span><span class="sxs-lookup"><span data-stu-id="cb2ec-137">Boolean</span></span>|<span data-ttu-id="cb2ec-138">Свойство, определяющее, включена ли языковая настройка в пользовательском потоке B2C.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-138">The property that determines whether language customization is enabled within the B2C user flow.</span></span> <span data-ttu-id="cb2ec-139">Настройка языка по умолчанию не включена для пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-139">Language customization is not enabled by default for B2C user flows.</span></span>|
|<span data-ttu-id="cb2ec-140">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="cb2ec-140">defaultLanguageTag</span></span>|<span data-ttu-id="cb2ec-141">Строка</span><span class="sxs-lookup"><span data-stu-id="cb2ec-141">String</span></span>|<span data-ttu-id="cb2ec-142">Указывает b2cIdentityUserFlow как язык по умолчанию, который используется, если в запросе не указан тег `ui_locale`.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-142">Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="cb2ec-143">Это поле соответствует спецификации [RFC 5646](https://tools.ietf.org/html/rfc5646).</span><span class="sxs-lookup"><span data-stu-id="cb2ec-143">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|

## <a name="response"></a><span data-ttu-id="cb2ec-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb2ec-144">Response</span></span>

<span data-ttu-id="cb2ec-145">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-145">If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb2ec-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb2ec-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb2ec-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb2ec-147">Request</span></span>

<span data-ttu-id="cb2ec-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cb2ec-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb2ec-149">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="cb2ec-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb2ec-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb2ec-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb2ec-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb2ec-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb2ec-152">Response</span></span>

<span data-ttu-id="cb2ec-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-153">The following is an example of the response.</span></span>

<span data-ttu-id="cb2ec-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cb2ec-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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
