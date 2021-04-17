---
title: Get identityUserFlowAttribute
description: Извлечение свойств и связей объекта identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 2396e09e10acdb82c914f888a2ebdada523da78a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882453"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="033c6-103">Get identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="033c6-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="033c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="033c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="033c6-105">Извлечение свойств и связей [объекта identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="033c6-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="033c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="033c6-106">Permissions</span></span>

<span data-ttu-id="033c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="033c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="033c6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="033c6-109">Permission type</span></span>      | <span data-ttu-id="033c6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="033c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="033c6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="033c6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="033c6-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="033c6-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="033c6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="033c6-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="033c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="033c6-114">Not supported.</span></span>|
|<span data-ttu-id="033c6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="033c6-115">Application</span></span>|<span data-ttu-id="033c6-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="033c6-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="033c6-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="033c6-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="033c6-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="033c6-118">Global administrator</span></span>
* <span data-ttu-id="033c6-119">Администратор атрибута потока внешних удостоверений</span><span class="sxs-lookup"><span data-stu-id="033c6-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="033c6-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="033c6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="033c6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="033c6-121">Request headers</span></span>

|<span data-ttu-id="033c6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="033c6-122">Name</span></span>|<span data-ttu-id="033c6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="033c6-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="033c6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="033c6-124">Authorization</span></span>|<span data-ttu-id="033c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="033c6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="033c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="033c6-127">Request body</span></span>

<span data-ttu-id="033c6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="033c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="033c6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="033c6-129">Response</span></span>

<span data-ttu-id="033c6-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON в тексте ответа [identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="033c6-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="033c6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="033c6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="033c6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="033c6-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/userFlowAttributes/{id}
```

### <a name="response"></a><span data-ttu-id="033c6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="033c6-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "City",
    "displayName": "City",
    "description": "Your city",
    "userFlowAttributeType": "builtIn",
    "dataType": "string"
}
```
