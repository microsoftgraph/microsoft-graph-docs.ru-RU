---
title: Get userFlowLanguageConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта userFlowLanguageConfiguration.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 054ed16948c86b872ee82572c770425e1c7b457b
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883026"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="0825a-103">Get userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="0825a-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="0825a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0825a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0825a-105">Ознакомьтесь с свойствами и отношениями [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0825a-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="0825a-106">Эти объекты представляют язык, доступный в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="0825a-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="0825a-107">**Примечание:** Настройка языка включена по умолчанию в [потоках пользователей Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="0825a-107">**Note:** Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0825a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0825a-108">Permissions</span></span>

<span data-ttu-id="0825a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0825a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0825a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0825a-111">Permission type</span></span>      | <span data-ttu-id="0825a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0825a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0825a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0825a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0825a-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0825a-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0825a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0825a-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0825a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0825a-116">Not supported.</span></span>|
|<span data-ttu-id="0825a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0825a-117">Application</span></span>|<span data-ttu-id="0825a-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0825a-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0825a-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="0825a-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0825a-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0825a-120">Global administrator</span></span>
* <span data-ttu-id="0825a-121">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="0825a-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0825a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0825a-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0825a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0825a-123">Request headers</span></span>

|<span data-ttu-id="0825a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0825a-124">Name</span></span>|<span data-ttu-id="0825a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0825a-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0825a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0825a-126">Authorization</span></span>|<span data-ttu-id="0825a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0825a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0825a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0825a-129">Request body</span></span>

<span data-ttu-id="0825a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0825a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0825a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0825a-131">Response</span></span>

<span data-ttu-id="0825a-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0825a-132">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0825a-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="0825a-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0825a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0825a-134">Request</span></span>

<span data-ttu-id="0825a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0825a-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en
```

### <a name="response"></a><span data-ttu-id="0825a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0825a-136">Response</span></span>

<span data-ttu-id="0825a-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0825a-137">The following is an example of the response.</span></span>

<span data-ttu-id="0825a-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0825a-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_Partner')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
