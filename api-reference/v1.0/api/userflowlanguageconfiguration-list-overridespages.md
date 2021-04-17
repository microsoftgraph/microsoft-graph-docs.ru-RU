---
title: Переопределения списка
description: Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5a1836288eda5a52f87bf168833ac4612a9c254e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883355"
---
# <a name="list-overridespages"></a><span data-ttu-id="06e56-103">Переопределения списка</span><span class="sxs-lookup"><span data-stu-id="06e56-103">List overridesPages</span></span>

<span data-ttu-id="06e56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06e56-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06e56-105">Получите ресурсы userFlowLanguagePage из свойства навигации overridesPages.</span><span class="sxs-lookup"><span data-stu-id="06e56-105">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="06e56-106">Эти страницы используются для настройки значений, показанных пользователю во время пользовательского пути в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="06e56-106">These pages are used to customize the values shown to the user during a user journey in a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="06e56-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06e56-107">Permissions</span></span>

<span data-ttu-id="06e56-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06e56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06e56-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06e56-110">Permission type</span></span>      | <span data-ttu-id="06e56-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06e56-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06e56-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06e56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06e56-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06e56-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="06e56-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06e56-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="06e56-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06e56-115">Not supported.</span></span>|
|<span data-ttu-id="06e56-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06e56-116">Application</span></span>|<span data-ttu-id="06e56-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06e56-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="06e56-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="06e56-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="06e56-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="06e56-119">Global administrator</span></span>
* <span data-ttu-id="06e56-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="06e56-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="06e56-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06e56-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages
```

## <a name="request-headers"></a><span data-ttu-id="06e56-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06e56-122">Request headers</span></span>

|<span data-ttu-id="06e56-123">Имя</span><span class="sxs-lookup"><span data-stu-id="06e56-123">Name</span></span>|<span data-ttu-id="06e56-124">Описание</span><span class="sxs-lookup"><span data-stu-id="06e56-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="06e56-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06e56-125">Authorization</span></span>|<span data-ttu-id="06e56-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06e56-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06e56-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06e56-128">Request body</span></span>

<span data-ttu-id="06e56-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06e56-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06e56-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="06e56-130">Response</span></span>

<span data-ttu-id="06e56-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06e56-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06e56-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="06e56-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06e56-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="06e56-133">Request</span></span>

<span data-ttu-id="06e56-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06e56-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_2"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages
```

### <a name="response"></a><span data-ttu-id="06e56-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="06e56-135">Response</span></span>

<span data-ttu-id="06e56-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06e56-136">The following is an example of the response.</span></span>

<span data-ttu-id="06e56-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06e56-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguagePage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "selfasserted1_1"
    }
  ]
}
```
