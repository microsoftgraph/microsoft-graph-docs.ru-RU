---
title: Список языков
description: Получить список языков, поддерживаемых для настройки в пользовательском потоке B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3b4ecc71cd37ca25a4d45b2cc65f1e6ef5cc4bbb
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706326"
---
# <a name="list-languages"></a><span data-ttu-id="1c000-103">Список языков</span><span class="sxs-lookup"><span data-stu-id="1c000-103">List languages</span></span>

<span data-ttu-id="1c000-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c000-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c000-105">Получить список языков, поддерживаемых для настройки в пользовательском потоке Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="1c000-105">Retrieve a list of languages supported for customization in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="1c000-106">**Примечание.** Чтобы получить список языков, поддерживаемых для настройки, необходимо сначала включить настройку языка в пользовательском потоке Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="1c000-106">**Note:** To retrieve a list of languages supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="1c000-107">Дополнительные сведения [см. в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="1c000-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c000-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c000-108">Permissions</span></span>

<span data-ttu-id="1c000-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c000-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c000-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c000-111">Permission type</span></span>      | <span data-ttu-id="1c000-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c000-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c000-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c000-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c000-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c000-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1c000-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c000-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1c000-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c000-116">Not supported.</span></span>|
|<span data-ttu-id="1c000-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1c000-117">Application</span></span>|<span data-ttu-id="1c000-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c000-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1c000-119">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="1c000-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1c000-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1c000-120">Global administrator</span></span>
* <span data-ttu-id="1c000-121">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="1c000-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1c000-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c000-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c000-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1c000-123">Optional query parameters</span></span>

<span data-ttu-id="1c000-124">Этот метод поддерживает параметр `$filter` запроса для показа только включенных языков.</span><span class="sxs-lookup"><span data-stu-id="1c000-124">This method supports the `$filter` query parameter to show only the enabled languages.</span></span> <span data-ttu-id="1c000-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1c000-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c000-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c000-126">Request headers</span></span>

|<span data-ttu-id="1c000-127">Имя</span><span class="sxs-lookup"><span data-stu-id="1c000-127">Name</span></span>|<span data-ttu-id="1c000-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1c000-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1c000-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c000-129">Authorization</span></span>|<span data-ttu-id="1c000-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c000-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c000-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c000-132">Request body</span></span>

<span data-ttu-id="1c000-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c000-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c000-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c000-134">Response</span></span>

<span data-ttu-id="1c000-135">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c000-135">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c000-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c000-136">Examples</span></span>

### <a name="example-1-retrieve-a-list-of-all-languages"></a><span data-ttu-id="1c000-137">Пример 1. Извлечение списка всех языков</span><span class="sxs-lookup"><span data-stu-id="1c000-137">Example 1: Retrieve a list of all languages</span></span>

#### <a name="request"></a><span data-ttu-id="1c000-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c000-138">Request</span></span>

<span data-ttu-id="1c000-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c000-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages
```

#### <a name="response"></a><span data-ttu-id="1c000-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c000-140">Response</span></span>

<span data-ttu-id="1c000-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c000-141">The following is an example of the response.</span></span>

<span data-ttu-id="1c000-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c000-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": false,
      "displayName": "Deutsch"
    }
  ]
}
```

### <a name="example-2-retrieve-a-list-of-only-enabled-languages"></a><span data-ttu-id="1c000-143">Пример 2. Извлечение списка только включенных языков</span><span class="sxs-lookup"><span data-stu-id="1c000-143">Example 2: Retrieve a list of only enabled languages</span></span>

#### <a name="request"></a><span data-ttu-id="1c000-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c000-144">Request</span></span>

<span data-ttu-id="1c000-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c000-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_filter"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages?$filter=isEnabled eq true
```

#### <a name="response"></a><span data-ttu-id="1c000-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c000-146">Response</span></span>

<span data-ttu-id="1c000-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c000-147">The following is an example of the response.</span></span>

<span data-ttu-id="1c000-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c000-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    }
  ]
}
```
