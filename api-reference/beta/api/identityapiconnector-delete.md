---
title: Удаление identityApiConnector
description: Удаляет объект identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da37c47620c82ee254b2e26ef97a72ecad4b8e3e
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720406"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="7e165-103">Удаление identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="7e165-103">Delete identityApiConnector</span></span>

<span data-ttu-id="7e165-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e165-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e165-105">Удаляет объект [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="7e165-105">Deletes an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e165-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e165-106">Permissions</span></span>

<span data-ttu-id="7e165-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e165-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e165-109">Permission type</span></span>                        | <span data-ttu-id="7e165-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e165-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7e165-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e165-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e165-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e165-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="7e165-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e165-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e165-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e165-114">Not supported.</span></span>  |
| <span data-ttu-id="7e165-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7e165-115">Application</span></span>                            | <span data-ttu-id="7e165-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e165-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="7e165-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="7e165-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7e165-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7e165-118">Global administrator</span></span>
* <span data-ttu-id="7e165-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="7e165-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7e165-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e165-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="7e165-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e165-121">Request headers</span></span>
|<span data-ttu-id="7e165-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7e165-122">Name</span></span>|<span data-ttu-id="7e165-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7e165-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7e165-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e165-124">Authorization</span></span>|<span data-ttu-id="7e165-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e165-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e165-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e165-127">Request body</span></span>
<span data-ttu-id="7e165-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e165-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e165-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e165-129">Response</span></span>

<span data-ttu-id="7e165-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7e165-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7e165-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e165-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e165-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e165-132">Request</span></span>

<span data-ttu-id="7e165-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e165-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```

### <a name="response"></a><span data-ttu-id="7e165-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e165-134">Response</span></span>

<span data-ttu-id="7e165-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e165-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
