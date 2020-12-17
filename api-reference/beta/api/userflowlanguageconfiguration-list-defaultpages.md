---
title: Список defaultPages
description: Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce8dca720388bd10c568aad950104a09cf268c7b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706422"
---
# <a name="list-defaultpages"></a><span data-ttu-id="6e9ec-103">Список defaultPages</span><span class="sxs-lookup"><span data-stu-id="6e9ec-103">List defaultPages</span></span>

<span data-ttu-id="6e9ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e9ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e9ec-105">Получите ресурсы userFlowLanguagePage из свойства навигации defaultPages.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-105">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="6e9ec-106">Они содержат значения, показанные пользователю в пользовательском пути по умолчанию для пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-106">These contain the values shown to the user in a default user journey of a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e9ec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e9ec-107">Permissions</span></span>

<span data-ttu-id="6e9ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e9ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e9ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e9ec-110">Permission type</span></span>      | <span data-ttu-id="6e9ec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e9ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e9ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e9ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e9ec-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e9ec-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="6e9ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e9ec-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6e9ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-115">Not supported.</span></span>|
|<span data-ttu-id="6e9ec-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e9ec-116">Application</span></span>|<span data-ttu-id="6e9ec-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e9ec-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="6e9ec-118">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="6e9ec-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="6e9ec-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6e9ec-119">Global administrator</span></span>
* <span data-ttu-id="6e9ec-120">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="6e9ec-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="6e9ec-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e9ec-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/defaultPages
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages
```

## <a name="request-headers"></a><span data-ttu-id="6e9ec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e9ec-122">Request headers</span></span>

|<span data-ttu-id="6e9ec-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6e9ec-123">Name</span></span>|<span data-ttu-id="6e9ec-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6e9ec-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e9ec-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e9ec-125">Authorization</span></span>|<span data-ttu-id="6e9ec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e9ec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e9ec-128">Request body</span></span>

<span data-ttu-id="6e9ec-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e9ec-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e9ec-130">Response</span></span>

<span data-ttu-id="6e9ec-131">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e9ec-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="6e9ec-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e9ec-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e9ec-133">Request</span></span>

<span data-ttu-id="6e9ec-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages
```

### <a name="response"></a><span data-ttu-id="6e9ec-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e9ec-135">Response</span></span>

<span data-ttu-id="6e9ec-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-136">The following is an example of the response.</span></span>

<span data-ttu-id="6e9ec-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6e9ec-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "idpselections"
    },
    {
      "id": "phonefactor"
    }
  ]
}
```
