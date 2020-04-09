---
title: Создание identityProvider
description: Создание объекта identityProvider
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6dec53d1a29ea4434169ccbc902c47691dc7b8b
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199867"
---
# <a name="create-identityprovider"></a><span data-ttu-id="22cf8-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="22cf8-103">Create identityProvider</span></span>

<span data-ttu-id="22cf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22cf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22cf8-105">Создание объекта [identityProvider](../resources/identityprovider.md) путем указания отображаемого имени, типа identityProvider, идентификатора клиента и секрета клиента.</span><span class="sxs-lookup"><span data-stu-id="22cf8-105">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="22cf8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22cf8-106">Permissions</span></span>

<span data-ttu-id="22cf8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22cf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22cf8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22cf8-109">Permission type</span></span>      | <span data-ttu-id="22cf8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22cf8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22cf8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22cf8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22cf8-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22cf8-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="22cf8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22cf8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="22cf8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22cf8-114">Not supported.</span></span>|
|<span data-ttu-id="22cf8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22cf8-115">Application</span></span>|<span data-ttu-id="22cf8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22cf8-116">Not supported.</span></span>|

<span data-ttu-id="22cf8-117">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="22cf8-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="22cf8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22cf8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="22cf8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22cf8-119">Request headers</span></span>

|<span data-ttu-id="22cf8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="22cf8-120">Name</span></span>|<span data-ttu-id="22cf8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="22cf8-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="22cf8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22cf8-122">Authorization</span></span>|<span data-ttu-id="22cf8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22cf8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="22cf8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22cf8-125">Content-Type</span></span>|<span data-ttu-id="22cf8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22cf8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22cf8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22cf8-128">Request body</span></span>

<span data-ttu-id="22cf8-129">Предоставьте в тексте запроса описание объекта [identityProvider](../resources/identityprovider.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22cf8-129">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="22cf8-130">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="22cf8-130">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="22cf8-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="22cf8-131">Property</span></span>|<span data-ttu-id="22cf8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="22cf8-132">Type</span></span>|<span data-ttu-id="22cf8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="22cf8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22cf8-134">clientId</span><span class="sxs-lookup"><span data-stu-id="22cf8-134">clientId</span></span>|<span data-ttu-id="22cf8-135">String</span><span class="sxs-lookup"><span data-stu-id="22cf8-135">String</span></span>|<span data-ttu-id="22cf8-136">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="22cf8-136">The client ID for the application.</span></span> <span data-ttu-id="22cf8-137">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="22cf8-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="22cf8-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="22cf8-138">clientSecret</span></span>|<span data-ttu-id="22cf8-139">String</span><span class="sxs-lookup"><span data-stu-id="22cf8-139">String</span></span>|<span data-ttu-id="22cf8-140">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="22cf8-140">The client secret for the application.</span></span> <span data-ttu-id="22cf8-141">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="22cf8-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="22cf8-142">name</span><span class="sxs-lookup"><span data-stu-id="22cf8-142">name</span></span>|<span data-ttu-id="22cf8-143">String</span><span class="sxs-lookup"><span data-stu-id="22cf8-143">String</span></span>|<span data-ttu-id="22cf8-144">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="22cf8-144">The display name of the identity provider.</span></span>|
|<span data-ttu-id="22cf8-145">type</span><span class="sxs-lookup"><span data-stu-id="22cf8-145">type</span></span>|<span data-ttu-id="22cf8-146">String</span><span class="sxs-lookup"><span data-stu-id="22cf8-146">String</span></span>|<span data-ttu-id="22cf8-147">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="22cf8-147">The identity provider type.</span></span> <span data-ttu-id="22cf8-148">Для сценариев B2C должно быть присвоено одно из указанных ниже значений.</span><span class="sxs-lookup"><span data-stu-id="22cf8-148">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="22cf8-149">Microsoft</span><span class="sxs-lookup"><span data-stu-id="22cf8-149">Microsoft</span></span><li/><span data-ttu-id="22cf8-150">Google</span><span class="sxs-lookup"><span data-stu-id="22cf8-150">Google</span></span><li/><span data-ttu-id="22cf8-151">Amazon</span><span class="sxs-lookup"><span data-stu-id="22cf8-151">Amazon</span></span><li/><span data-ttu-id="22cf8-152">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="22cf8-152">LinkedIn</span></span><li/><span data-ttu-id="22cf8-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="22cf8-153">Facebook</span></span><li/><span data-ttu-id="22cf8-154">GitHub</span><span class="sxs-lookup"><span data-stu-id="22cf8-154">GitHub</span></span><li/><span data-ttu-id="22cf8-155">Twitter</span><span class="sxs-lookup"><span data-stu-id="22cf8-155">Twitter</span></span><li/><span data-ttu-id="22cf8-156">Weibo</span><span class="sxs-lookup"><span data-stu-id="22cf8-156">Weibo</span></span><li/><span data-ttu-id="22cf8-157">QQ</span><span class="sxs-lookup"><span data-stu-id="22cf8-157">QQ</span></span><li/><span data-ttu-id="22cf8-158">WeChat</span><span class="sxs-lookup"><span data-stu-id="22cf8-158">WeChat</span></span></ul><span data-ttu-id="22cf8-159">Для сценариев B2B можно использовать только Google</span><span class="sxs-lookup"><span data-stu-id="22cf8-159">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="22cf8-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="22cf8-160">Response</span></span>

<span data-ttu-id="22cf8-161">В случае успеха этот метод возвращает код отклика `201 Created` и объект [identityProvider](../resources/identityprovider.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22cf8-161">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="22cf8-162">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="22cf8-162">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="22cf8-163">Пример</span><span class="sxs-lookup"><span data-stu-id="22cf8-163">Example</span></span>

<span data-ttu-id="22cf8-164">В приведенном ниже примере создается объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="22cf8-164">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="22cf8-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="22cf8-165">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="22cf8-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="22cf8-166">Response</span></span>

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


