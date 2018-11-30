---
title: Создание identityProvider
description: Создайте новый identityProvider, указав отображаемое имя, тип identityProvider, идентификатор клиента и секрет клиента.
ms.openlocfilehash: 8786cbf6676567a0c6aaef5bf497f50cff1ce9a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079359"
---
# <a name="create-identityprovider"></a><span data-ttu-id="29390-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="29390-103">Create identityProvider</span></span>

> <span data-ttu-id="29390-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29390-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29390-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29390-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29390-106">Создайте новый [identityProvider](../resources/identityprovider.md) , указав отображаемое имя, тип identityProvider, идентификатор клиента и секрет клиента.</span><span class="sxs-lookup"><span data-stu-id="29390-106">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="29390-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29390-107">Permissions</span></span>

<span data-ttu-id="29390-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29390-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29390-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29390-110">Permission type</span></span>      | <span data-ttu-id="29390-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29390-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29390-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29390-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29390-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29390-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="29390-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29390-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="29390-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29390-115">Not supported.</span></span>|
|<span data-ttu-id="29390-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29390-116">Application</span></span>|<span data-ttu-id="29390-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29390-117">Not supported.</span></span>|

<span data-ttu-id="29390-118">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="29390-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="29390-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29390-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="29390-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29390-120">Request headers</span></span>

|<span data-ttu-id="29390-121">Имя</span><span class="sxs-lookup"><span data-stu-id="29390-121">Name</span></span>|<span data-ttu-id="29390-122">Описание</span><span class="sxs-lookup"><span data-stu-id="29390-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="29390-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29390-123">Authorization</span></span>|<span data-ttu-id="29390-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29390-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="29390-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29390-126">Content-Type</span></span>|<span data-ttu-id="29390-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29390-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29390-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29390-129">Request body</span></span>

<span data-ttu-id="29390-130">В тексте запроса для представления JSON объекта [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="29390-130">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="29390-131">Требуются все свойства, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="29390-131">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="29390-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="29390-132">Property</span></span>|<span data-ttu-id="29390-133">Тип</span><span class="sxs-lookup"><span data-stu-id="29390-133">Type</span></span>|<span data-ttu-id="29390-134">Description</span><span class="sxs-lookup"><span data-stu-id="29390-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29390-135">clientId</span><span class="sxs-lookup"><span data-stu-id="29390-135">clientId</span></span>|<span data-ttu-id="29390-136">String</span><span class="sxs-lookup"><span data-stu-id="29390-136">String</span></span>|<span data-ttu-id="29390-137">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="29390-137">The client ID for the application.</span></span> <span data-ttu-id="29390-138">Это идентификатор клиента, полученные при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="29390-138">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="29390-139">clientSecret</span><span class="sxs-lookup"><span data-stu-id="29390-139">clientSecret</span></span>|<span data-ttu-id="29390-140">String</span><span class="sxs-lookup"><span data-stu-id="29390-140">String</span></span>|<span data-ttu-id="29390-141">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="29390-141">The client secret for the application.</span></span> <span data-ttu-id="29390-142">Это секрет клиента, полученные при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="29390-142">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="29390-143">name</span><span class="sxs-lookup"><span data-stu-id="29390-143">name</span></span>|<span data-ttu-id="29390-144">String</span><span class="sxs-lookup"><span data-stu-id="29390-144">String</span></span>|<span data-ttu-id="29390-145">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="29390-145">The display name of the identity provider.</span></span>|
|<span data-ttu-id="29390-146">type</span><span class="sxs-lookup"><span data-stu-id="29390-146">type</span></span>|<span data-ttu-id="29390-147">String</span><span class="sxs-lookup"><span data-stu-id="29390-147">String</span></span>|<span data-ttu-id="29390-148">Тип поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="29390-148">The identity provider type.</span></span> <span data-ttu-id="29390-149">Оно должно быть одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="29390-149">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="29390-150">Microsoft</span><span class="sxs-lookup"><span data-stu-id="29390-150">Microsoft</span></span><li/><span data-ttu-id="29390-151">Google</span><span class="sxs-lookup"><span data-stu-id="29390-151">Google</span></span><li/><span data-ttu-id="29390-152">Amazon</span><span class="sxs-lookup"><span data-stu-id="29390-152">Amazon</span></span><li/><span data-ttu-id="29390-153">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="29390-153">LinkedIn</span></span><li/><span data-ttu-id="29390-154">Facebook</span><span class="sxs-lookup"><span data-stu-id="29390-154">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="29390-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="29390-155">Response</span></span>

<span data-ttu-id="29390-156">Успешно завершена, этот метод возвращает `201 Created` объект [identityProvider](../resources/identityprovider.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="29390-156">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="29390-157">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="29390-157">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="29390-158">Пример</span><span class="sxs-lookup"><span data-stu-id="29390-158">Example</span></span>

<span data-ttu-id="29390-159">В следующем примере создается **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="29390-159">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="29390-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="29390-160">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="29390-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="29390-161">Response</span></span>

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
