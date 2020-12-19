---
title: Список identityApiConnectors
description: Получить список объектов identityApiConnector и их свойств
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ca946e80b590926aa8f15b7b790d5bd098838cf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720401"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="111ef-103">Список identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="111ef-103">List identityApiConnectors</span></span>

<span data-ttu-id="111ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="111ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="111ef-105">Чтение свойств объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="111ef-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="111ef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="111ef-106">Permissions</span></span>

<span data-ttu-id="111ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="111ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="111ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="111ef-109">Permission type</span></span>                        | <span data-ttu-id="111ef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="111ef-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="111ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="111ef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="111ef-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="111ef-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="111ef-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="111ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="111ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="111ef-114">Not supported.</span></span>  |
| <span data-ttu-id="111ef-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="111ef-115">Application</span></span>                            | <span data-ttu-id="111ef-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="111ef-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="111ef-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="111ef-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="111ef-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="111ef-118">Global administrator</span></span>
* <span data-ttu-id="111ef-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="111ef-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="111ef-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="111ef-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="111ef-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="111ef-121">Optional query parameters</span></span>
<span data-ttu-id="111ef-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="111ef-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="111ef-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="111ef-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="111ef-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="111ef-124">Request headers</span></span>
|<span data-ttu-id="111ef-125">Имя</span><span class="sxs-lookup"><span data-stu-id="111ef-125">Name</span></span>|<span data-ttu-id="111ef-126">Описание</span><span class="sxs-lookup"><span data-stu-id="111ef-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="111ef-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="111ef-127">Authorization</span></span>|<span data-ttu-id="111ef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="111ef-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="111ef-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="111ef-130">Request body</span></span>
<span data-ttu-id="111ef-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="111ef-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="111ef-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="111ef-132">Response</span></span>

<span data-ttu-id="111ef-133">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [identityApiConnector](../resources/identityapiconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="111ef-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="111ef-134">Пример</span><span class="sxs-lookup"><span data-stu-id="111ef-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="111ef-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="111ef-135">Request</span></span>

<span data-ttu-id="111ef-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="111ef-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```

### <a name="response"></a><span data-ttu-id="111ef-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="111ef-137">Response</span></span>

<span data-ttu-id="111ef-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="111ef-138">The following is an example of the response.</span></span>

<span data-ttu-id="111ef-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="111ef-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors",
    "value": [
      {
          "id": "<guid>",
          "displayName": "Test API",
          "targetUrl": "https://someapi.com/api/endpoint",
          "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME>",
            "password": "******"
          }
      }
  ]
}
```
