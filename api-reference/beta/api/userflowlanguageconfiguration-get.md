---
title: Get userFlowLanguageConfiguration
description: Чтение свойств и связей объекта [userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d25533822a5f67cdfc98564a41e7f53b3be98208
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706397"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="883c6-103">Get userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="883c6-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="883c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="883c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="883c6-105">Чтение свойств и связей объекта [userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="883c6-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="883c6-106">Эти объекты представляют язык, доступный в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="883c6-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="883c6-107">**Примечание.** Чтобы получить язык, поддерживаемый для настройки, необходимо сначала включить настройку языка в пользовательском потоке B2C Azure AD.</span><span class="sxs-lookup"><span data-stu-id="883c6-107">**Note:** To retrieve a language supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="883c6-108">Дополнительные сведения [см. в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="883c6-108">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span> <span data-ttu-id="883c6-109">Настройка языка включена по умолчанию в потоках пользователей [Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="883c6-109">Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="883c6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="883c6-110">Permissions</span></span>

<span data-ttu-id="883c6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="883c6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="883c6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="883c6-113">Permission type</span></span>      | <span data-ttu-id="883c6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="883c6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="883c6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="883c6-115">Delegated (work or school account)</span></span>|<span data-ttu-id="883c6-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="883c6-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="883c6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="883c6-117">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="883c6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="883c6-118">Not supported.</span></span>|
|<span data-ttu-id="883c6-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="883c6-119">Application</span></span>|<span data-ttu-id="883c6-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="883c6-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="883c6-121">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="883c6-121">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="883c6-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="883c6-122">Global administrator</span></span>
* <span data-ttu-id="883c6-123">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="883c6-123">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="883c6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="883c6-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/languages/{id}
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="883c6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="883c6-125">Request headers</span></span>

|<span data-ttu-id="883c6-126">Имя</span><span class="sxs-lookup"><span data-stu-id="883c6-126">Name</span></span>|<span data-ttu-id="883c6-127">Описание</span><span class="sxs-lookup"><span data-stu-id="883c6-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="883c6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="883c6-128">Authorization</span></span>|<span data-ttu-id="883c6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="883c6-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="883c6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="883c6-131">Request body</span></span>

<span data-ttu-id="883c6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="883c6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="883c6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="883c6-133">Response</span></span>

<span data-ttu-id="883c6-134">В случае успеха этот метод возвращает код отклика и объект `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="883c6-134">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="883c6-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="883c6-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="883c6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="883c6-136">Request</span></span>

<span data-ttu-id="883c6-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="883c6-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en
```

### <a name="response"></a><span data-ttu-id="883c6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="883c6-138">Response</span></span>

<span data-ttu-id="883c6-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="883c6-139">The following is an example of the response.</span></span>

<span data-ttu-id="883c6-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="883c6-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_Customer')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
