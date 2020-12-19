---
title: Создание identityApiConnector
description: Создание объекта identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6665054307d601e80d02402a188f6412ab923ffc
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720407"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="91c56-103">Создание identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="91c56-103">Create identityApiConnector</span></span>

<span data-ttu-id="91c56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91c56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91c56-105">Создание объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="91c56-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91c56-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91c56-106">Permissions</span></span>

<span data-ttu-id="91c56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91c56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91c56-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91c56-109">Permission type</span></span>                        | <span data-ttu-id="91c56-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91c56-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="91c56-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91c56-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91c56-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91c56-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="91c56-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91c56-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91c56-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91c56-114">Not supported.</span></span>  |
| <span data-ttu-id="91c56-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="91c56-115">Application</span></span>                            | <span data-ttu-id="91c56-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91c56-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="91c56-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="91c56-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="91c56-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="91c56-118">Global administrator</span></span>
* <span data-ttu-id="91c56-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="91c56-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="91c56-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91c56-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="91c56-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91c56-121">Request headers</span></span>

| <span data-ttu-id="91c56-122">Имя</span><span class="sxs-lookup"><span data-stu-id="91c56-122">Name</span></span>          | <span data-ttu-id="91c56-123">Описание</span><span class="sxs-lookup"><span data-stu-id="91c56-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="91c56-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91c56-124">Authorization</span></span> | <span data-ttu-id="91c56-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91c56-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="91c56-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91c56-127">Content-Type</span></span>  | <span data-ttu-id="91c56-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91c56-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91c56-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91c56-130">Request body</span></span>

<span data-ttu-id="91c56-131">В теле запроса укажу представление объекта [identityApiConnector](../resources/identityapiconnector.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="91c56-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="91c56-132">В следующей таблице показаны свойства, необходимые при создании [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="91c56-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="91c56-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="91c56-133">Property</span></span>|<span data-ttu-id="91c56-134">Тип</span><span class="sxs-lookup"><span data-stu-id="91c56-134">Type</span></span>|<span data-ttu-id="91c56-135">Описание</span><span class="sxs-lookup"><span data-stu-id="91c56-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91c56-136">displayName</span><span class="sxs-lookup"><span data-stu-id="91c56-136">displayName</span></span>|<span data-ttu-id="91c56-137">String</span><span class="sxs-lookup"><span data-stu-id="91c56-137">String</span></span>| <span data-ttu-id="91c56-138">Имя соединители API.</span><span class="sxs-lookup"><span data-stu-id="91c56-138">The name of the API connector.</span></span> |
|<span data-ttu-id="91c56-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="91c56-139">targetUrl</span></span>|<span data-ttu-id="91c56-140">String</span><span class="sxs-lookup"><span data-stu-id="91c56-140">String</span></span>| <span data-ttu-id="91c56-141">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="91c56-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="91c56-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="91c56-142">authenticationConfiguration</span></span>|[<span data-ttu-id="91c56-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="91c56-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="91c56-144">Объект, который описывает сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="91c56-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="91c56-145">Поддерживается [только базовая](../resources/basicauthentication.md) проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="91c56-145">Only [Basic authentication](../resources/basicauthentication.md) is supported.</span></span>|

## <a name="response"></a><span data-ttu-id="91c56-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="91c56-146">Response</span></span>

<span data-ttu-id="91c56-147">В случае успеха этот метод возвращает код отклика и объект `201 Created` [identityApiConnector](../resources/identityapiconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91c56-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91c56-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="91c56-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91c56-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="91c56-149">Request</span></span>

<span data-ttu-id="91c56-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91c56-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/beta/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username":"<USERNAME>",
      "password":"<PASSWORD>"
    }
}
```

### <a name="response"></a><span data-ttu-id="91c56-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="91c56-151">Response</span></span>

<span data-ttu-id="91c56-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91c56-152">The following is an example of the response.</span></span>

<span data-ttu-id="91c56-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="91c56-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
