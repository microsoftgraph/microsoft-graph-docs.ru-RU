---
title: Создание identityProvider
description: Создание объекта identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ffd1f600395a1c72f2ab4c72ef1c3d3a358e387
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016155"
---
# <a name="create-identityprovider"></a><span data-ttu-id="964c3-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="964c3-103">Create identityProvider</span></span>

<span data-ttu-id="964c3-104">Создание объекта [identityProvider](../resources/identityprovider.md) путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.</span><span class="sxs-lookup"><span data-stu-id="964c3-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="964c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="964c3-105">Permissions</span></span>

<span data-ttu-id="964c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="964c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="964c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="964c3-108">Permission type</span></span>      | <span data-ttu-id="964c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="964c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="964c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="964c3-110">Delegated (work or school account)</span></span>|<span data-ttu-id="964c3-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="964c3-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="964c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="964c3-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="964c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="964c3-113">Not supported.</span></span>|
|<span data-ttu-id="964c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="964c3-114">Application</span></span>|<span data-ttu-id="964c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="964c3-115">Not supported.</span></span>|

<span data-ttu-id="964c3-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="964c3-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="964c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="964c3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="964c3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="964c3-118">Request headers</span></span>

|<span data-ttu-id="964c3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="964c3-119">Name</span></span>|<span data-ttu-id="964c3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="964c3-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="964c3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="964c3-121">Authorization</span></span>|<span data-ttu-id="964c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="964c3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="964c3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="964c3-124">Content-Type</span></span>|<span data-ttu-id="964c3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="964c3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="964c3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="964c3-127">Request body</span></span>

<span data-ttu-id="964c3-128">Предоставьте в тексте запроса описание объекта [identityProvider](../resources/identityprovider.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="964c3-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="964c3-129">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="964c3-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="964c3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="964c3-130">Property</span></span>|<span data-ttu-id="964c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="964c3-131">Type</span></span>|<span data-ttu-id="964c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="964c3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="964c3-133">clientId</span><span class="sxs-lookup"><span data-stu-id="964c3-133">clientId</span></span>|<span data-ttu-id="964c3-134">String</span><span class="sxs-lookup"><span data-stu-id="964c3-134">String</span></span>|<span data-ttu-id="964c3-135">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="964c3-135">The client ID for the application.</span></span> <span data-ttu-id="964c3-136">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="964c3-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="964c3-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="964c3-137">clientSecret</span></span>|<span data-ttu-id="964c3-138">String</span><span class="sxs-lookup"><span data-stu-id="964c3-138">String</span></span>|<span data-ttu-id="964c3-139">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="964c3-139">The client secret for the application.</span></span> <span data-ttu-id="964c3-140">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="964c3-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="964c3-141">name</span><span class="sxs-lookup"><span data-stu-id="964c3-141">name</span></span>|<span data-ttu-id="964c3-142">String</span><span class="sxs-lookup"><span data-stu-id="964c3-142">String</span></span>|<span data-ttu-id="964c3-143">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="964c3-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="964c3-144">type</span><span class="sxs-lookup"><span data-stu-id="964c3-144">type</span></span>|<span data-ttu-id="964c3-145">String</span><span class="sxs-lookup"><span data-stu-id="964c3-145">String</span></span>|<span data-ttu-id="964c3-146">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="964c3-146">The identity provider type.</span></span> <span data-ttu-id="964c3-147">Для сценариев B2C должно быть присвоено одно из указанных ниже значений.</span><span class="sxs-lookup"><span data-stu-id="964c3-147">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="964c3-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="964c3-148">Microsoft</span></span><li/><span data-ttu-id="964c3-149">Google</span><span class="sxs-lookup"><span data-stu-id="964c3-149">Google</span></span><li/><span data-ttu-id="964c3-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="964c3-150">Amazon</span></span><li/><span data-ttu-id="964c3-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="964c3-151">LinkedIn</span></span><li/><span data-ttu-id="964c3-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="964c3-152">Facebook</span></span><li/><span data-ttu-id="964c3-153">GitHub</span><span class="sxs-lookup"><span data-stu-id="964c3-153">GitHub</span></span><li/><span data-ttu-id="964c3-154">Twitter</span><span class="sxs-lookup"><span data-stu-id="964c3-154">Twitter</span></span><li/><span data-ttu-id="964c3-155">Weibo</span><span class="sxs-lookup"><span data-stu-id="964c3-155">Weibo</span></span><li/><span data-ttu-id="964c3-156">QQ</span><span class="sxs-lookup"><span data-stu-id="964c3-156">QQ</span></span><li/><span data-ttu-id="964c3-157">WeChat</span><span class="sxs-lookup"><span data-stu-id="964c3-157">WeChat</span></span></ul><span data-ttu-id="964c3-158">Для сценариев B2B можно использовать только Google</span><span class="sxs-lookup"><span data-stu-id="964c3-158">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="964c3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="964c3-159">Response</span></span>

<span data-ttu-id="964c3-160">В случае успеха этот метод возвращает код отклика `201 Created` и объект [identityProvider](../resources/identityprovider.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="964c3-160">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="964c3-161">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="964c3-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="964c3-162">Пример</span><span class="sxs-lookup"><span data-stu-id="964c3-162">Example</span></span>

<span data-ttu-id="964c3-163">В приведенном ниже примере создается объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="964c3-163">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="964c3-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="964c3-164">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="964c3-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="964c3-165">Response</span></span>

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


