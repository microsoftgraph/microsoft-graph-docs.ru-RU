---
title: Создание identityProvider
description: Создание объекта identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a33354c35903fedc3efedb84e9f2ed7bc20c9506
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649449"
---
# <a name="create-identityprovider"></a><span data-ttu-id="5d4cb-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="5d4cb-103">Create identityProvider</span></span>

<span data-ttu-id="5d4cb-104">Создание объекта [identityProvider](../resources/identityprovider.md) путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d4cb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d4cb-105">Permissions</span></span>

<span data-ttu-id="5d4cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d4cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d4cb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d4cb-108">Permission type</span></span>      | <span data-ttu-id="5d4cb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d4cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d4cb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d4cb-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5d4cb-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d4cb-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="5d4cb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d4cb-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5d4cb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-113">Not supported.</span></span>|
|<span data-ttu-id="5d4cb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d4cb-114">Application</span></span>|<span data-ttu-id="5d4cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-115">Not supported.</span></span>|

<span data-ttu-id="5d4cb-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="5d4cb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d4cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="5d4cb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d4cb-118">Request headers</span></span>

|<span data-ttu-id="5d4cb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d4cb-119">Name</span></span>|<span data-ttu-id="5d4cb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5d4cb-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5d4cb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d4cb-121">Authorization</span></span>|<span data-ttu-id="5d4cb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5d4cb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d4cb-124">Content-Type</span></span>|<span data-ttu-id="5d4cb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d4cb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d4cb-127">Request body</span></span>

<span data-ttu-id="5d4cb-128">Предоставьте в тексте запроса описание объекта [identityProvider](../resources/identityProvider.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-128">In the request body, supply a JSON representation of a [team](../resources/identityProvider.md) object.</span></span> <span data-ttu-id="5d4cb-129">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="5d4cb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d4cb-130">Property</span></span>|<span data-ttu-id="5d4cb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5d4cb-131">Type</span></span>|<span data-ttu-id="5d4cb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5d4cb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d4cb-133">clientId</span><span class="sxs-lookup"><span data-stu-id="5d4cb-133">clientId</span></span>|<span data-ttu-id="5d4cb-134">String</span><span class="sxs-lookup"><span data-stu-id="5d4cb-134">String</span></span>|<span data-ttu-id="5d4cb-135">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-135">The client ID created for your application.</span></span> <span data-ttu-id="5d4cb-136">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="5d4cb-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="5d4cb-137">client_secret</span></span>|<span data-ttu-id="5d4cb-138">String</span><span class="sxs-lookup"><span data-stu-id="5d4cb-138">String</span></span>|<span data-ttu-id="5d4cb-139">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-139">The client secret created for your application.</span></span> <span data-ttu-id="5d4cb-140">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="5d4cb-141">name</span><span class="sxs-lookup"><span data-stu-id="5d4cb-141">name</span></span>|<span data-ttu-id="5d4cb-142">String</span><span class="sxs-lookup"><span data-stu-id="5d4cb-142">String</span></span>|<span data-ttu-id="5d4cb-143">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-143">The unique name of the identity provider.</span></span>|
|<span data-ttu-id="5d4cb-144">type</span><span class="sxs-lookup"><span data-stu-id="5d4cb-144">type</span></span>|<span data-ttu-id="5d4cb-145">String</span><span class="sxs-lookup"><span data-stu-id="5d4cb-145">String</span></span>|<span data-ttu-id="5d4cb-146">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="5d4cb-146">The identity provider type.</span></span> <span data-ttu-id="5d4cb-147">Для сценариев B2C должно быть присвоено одно из указанных ниже значений.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-147">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="5d4cb-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="5d4cb-148">Microsoft</span></span><li/><span data-ttu-id="5d4cb-149">Google</span><span class="sxs-lookup"><span data-stu-id="5d4cb-149">Google</span></span><li/><span data-ttu-id="5d4cb-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="5d4cb-150">Amazon</span></span><li/><span data-ttu-id="5d4cb-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="5d4cb-151">LinkedIn</span></span><li/><span data-ttu-id="5d4cb-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="5d4cb-152">Facebook</span></span><li/><span data-ttu-id="5d4cb-153">GitHub</span><span class="sxs-lookup"><span data-stu-id="5d4cb-153">GitHub</span></span><li/><span data-ttu-id="5d4cb-154">Twitter</span><span class="sxs-lookup"><span data-stu-id="5d4cb-154">Twitter</span></span><li/><span data-ttu-id="5d4cb-155">Weibo</span><span class="sxs-lookup"><span data-stu-id="5d4cb-155">Weibo</span></span><li/><span data-ttu-id="5d4cb-156">QQ</span><span class="sxs-lookup"><span data-stu-id="5d4cb-156">QQ</span></span><li/><span data-ttu-id="5d4cb-157">WeChat</span><span class="sxs-lookup"><span data-stu-id="5d4cb-157">WeChat</span></span></ul><span data-ttu-id="5d4cb-158">Для сценариев B2B можно использовать только Google</span><span class="sxs-lookup"><span data-stu-id="5d4cb-158">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="5d4cb-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d4cb-159">Response</span></span>

<span data-ttu-id="5d4cb-160">В случае успеха этот метод возвращает код отклика `201 Created` и объект [identityProvider](../resources/identityProvider.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-160">If successful, this method returns a `201 Created` response code and [Contract](../resources/identityProvider.md) object in the response body.</span></span> <span data-ttu-id="5d4cb-161">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="5d4cb-162">Пример</span><span class="sxs-lookup"><span data-stu-id="5d4cb-162">Example</span></span>

<span data-ttu-id="5d4cb-163">В приведенном ниже примере создается объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="5d4cb-163">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="5d4cb-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d4cb-164">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="5d4cb-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d4cb-165">Response</span></span>

<!-- { "blockType": "ignored" } -->
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


