---
title: List identityUserFlowAttributes
description: Извлечение списка объектов identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4d0a596f8710d319f5c57e651e1fa59a997e88b2
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882458"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="63337-103">List identityUserFlowAttributes</span><span class="sxs-lookup"><span data-stu-id="63337-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="63337-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63337-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63337-105">Извлечение списка [объектов identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="63337-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="63337-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63337-106">Permissions</span></span>

<span data-ttu-id="63337-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63337-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63337-109">Permission type</span></span>      | <span data-ttu-id="63337-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63337-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63337-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63337-111">Delegated (work or school account)</span></span>|<span data-ttu-id="63337-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63337-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="63337-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63337-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="63337-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63337-114">Not supported.</span></span>|
|<span data-ttu-id="63337-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63337-115">Application</span></span>|<span data-ttu-id="63337-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63337-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="63337-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="63337-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="63337-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="63337-118">Global administrator</span></span>
* <span data-ttu-id="63337-119">Администратор атрибута потока внешних удостоверений</span><span class="sxs-lookup"><span data-stu-id="63337-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="63337-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63337-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="63337-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63337-121">Request headers</span></span>

|<span data-ttu-id="63337-122">Имя</span><span class="sxs-lookup"><span data-stu-id="63337-122">Name</span></span>|<span data-ttu-id="63337-123">Описание</span><span class="sxs-lookup"><span data-stu-id="63337-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="63337-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63337-124">Authorization</span></span>|<span data-ttu-id="63337-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63337-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63337-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63337-127">Request body</span></span>

<span data-ttu-id="63337-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63337-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63337-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="63337-129">Response</span></span>

<span data-ttu-id="63337-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="63337-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63337-131">Пример</span><span class="sxs-lookup"><span data-stu-id="63337-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63337-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="63337-132">Request</span></span>

<span data-ttu-id="63337-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63337-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/userFlowAttributes
```

### <a name="response"></a><span data-ttu-id="63337-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="63337-134">Response</span></span>

<span data-ttu-id="63337-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63337-135">The following is an example of the response.</span></span>

<span data-ttu-id="63337-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63337-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#userFlowAttributes",
    "value": [
      {
          "id": "City",
          "displayName": "City",
          "description": "Your city",
          "userFlowAttributeType": "builtIn",
          "dataType": "string"
      },
      {
          "id": "extension_d09380e2b4c6429a203fb816a04a7ad_Hobby",
          "displayName": "Hobby",
          "description": "Your hobby",
          "userFlowAttributeType": "custom",
          "dataType": "string",
      },
    ]
}
```
