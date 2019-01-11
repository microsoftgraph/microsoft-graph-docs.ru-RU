---
title: Создание identityProvider
description: Создайте новый identityProvider, указав отображаемое имя, тип identityProvider, идентификатор клиента и секрет клиента.
localization_priority: Normal
ms.openlocfilehash: 50ead5acbbda7725e44de55865d6fe2184c89647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866236"
---
# <a name="create-identityprovider"></a><span data-ttu-id="50e31-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="50e31-103">Create identityProvider</span></span>

> <span data-ttu-id="50e31-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50e31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50e31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50e31-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50e31-106">Создайте новый [identityProvider](../resources/identityprovider.md) , указав отображаемое имя, тип identityProvider, идентификатор клиента и секрет клиента.</span><span class="sxs-lookup"><span data-stu-id="50e31-106">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="50e31-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50e31-107">Permissions</span></span>

<span data-ttu-id="50e31-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50e31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50e31-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50e31-110">Permission type</span></span>      | <span data-ttu-id="50e31-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50e31-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50e31-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50e31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50e31-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50e31-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="50e31-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50e31-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="50e31-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50e31-115">Not supported.</span></span>|
|<span data-ttu-id="50e31-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50e31-116">Application</span></span>|<span data-ttu-id="50e31-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50e31-117">Not supported.</span></span>|

<span data-ttu-id="50e31-118">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="50e31-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="50e31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50e31-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="50e31-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50e31-120">Request headers</span></span>

|<span data-ttu-id="50e31-121">Имя</span><span class="sxs-lookup"><span data-stu-id="50e31-121">Name</span></span>|<span data-ttu-id="50e31-122">Описание</span><span class="sxs-lookup"><span data-stu-id="50e31-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="50e31-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50e31-123">Authorization</span></span>|<span data-ttu-id="50e31-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50e31-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="50e31-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50e31-126">Content-Type</span></span>|<span data-ttu-id="50e31-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50e31-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50e31-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50e31-129">Request body</span></span>

<span data-ttu-id="50e31-130">В тексте запроса для представления JSON объекта [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="50e31-130">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="50e31-131">Требуются все свойства, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="50e31-131">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="50e31-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="50e31-132">Property</span></span>|<span data-ttu-id="50e31-133">Тип</span><span class="sxs-lookup"><span data-stu-id="50e31-133">Type</span></span>|<span data-ttu-id="50e31-134">Описание</span><span class="sxs-lookup"><span data-stu-id="50e31-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50e31-135">clientId</span><span class="sxs-lookup"><span data-stu-id="50e31-135">clientId</span></span>|<span data-ttu-id="50e31-136">Строка</span><span class="sxs-lookup"><span data-stu-id="50e31-136">String</span></span>|<span data-ttu-id="50e31-137">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="50e31-137">The client ID for the application.</span></span> <span data-ttu-id="50e31-138">Это идентификатор клиента, полученные при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="50e31-138">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="50e31-139">clientSecret</span><span class="sxs-lookup"><span data-stu-id="50e31-139">clientSecret</span></span>|<span data-ttu-id="50e31-140">Строка</span><span class="sxs-lookup"><span data-stu-id="50e31-140">String</span></span>|<span data-ttu-id="50e31-141">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="50e31-141">The client secret for the application.</span></span> <span data-ttu-id="50e31-142">Это секрет клиента, полученные при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="50e31-142">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="50e31-143">name</span><span class="sxs-lookup"><span data-stu-id="50e31-143">name</span></span>|<span data-ttu-id="50e31-144">Строка</span><span class="sxs-lookup"><span data-stu-id="50e31-144">String</span></span>|<span data-ttu-id="50e31-145">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="50e31-145">The display name of the identity provider.</span></span>|
|<span data-ttu-id="50e31-146">type</span><span class="sxs-lookup"><span data-stu-id="50e31-146">type</span></span>|<span data-ttu-id="50e31-147">Строка</span><span class="sxs-lookup"><span data-stu-id="50e31-147">String</span></span>|<span data-ttu-id="50e31-148">Тип поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="50e31-148">The identity provider type.</span></span> <span data-ttu-id="50e31-149">Оно должно быть одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="50e31-149">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="50e31-150">Microsoft</span><span class="sxs-lookup"><span data-stu-id="50e31-150">Microsoft</span></span><li/><span data-ttu-id="50e31-151">Google</span><span class="sxs-lookup"><span data-stu-id="50e31-151">Google</span></span><li/><span data-ttu-id="50e31-152">Amazon</span><span class="sxs-lookup"><span data-stu-id="50e31-152">Amazon</span></span><li/><span data-ttu-id="50e31-153">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="50e31-153">LinkedIn</span></span><li/><span data-ttu-id="50e31-154">Facebook</span><span class="sxs-lookup"><span data-stu-id="50e31-154">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="50e31-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="50e31-155">Response</span></span>

<span data-ttu-id="50e31-156">Успешно завершена, этот метод возвращает `201 Created` объект [identityProvider](../resources/identityprovider.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="50e31-156">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="50e31-157">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="50e31-157">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="50e31-158">Пример</span><span class="sxs-lookup"><span data-stu-id="50e31-158">Example</span></span>

<span data-ttu-id="50e31-159">В следующем примере создается **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="50e31-159">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="50e31-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="50e31-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="50e31-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="50e31-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
