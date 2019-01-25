---
title: Создание identityProvider
description: Создайте новый identityProvider, указав отображаемое имя, тип identityProvider, идентификатор клиента и секрет клиента.
localization_priority: Normal
ms.openlocfilehash: c0b005d729510fa68d9edd8bfea7b85687543cf2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514651"
---
# <a name="create-identityprovider"></a><span data-ttu-id="349f1-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="349f1-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="349f1-104">Создайте новый [identityProvider](../resources/identityprovider.md) , указав отображаемое имя, тип identityProvider, идентификатор клиента и секрет клиента.</span><span class="sxs-lookup"><span data-stu-id="349f1-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="349f1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="349f1-105">Permissions</span></span>

<span data-ttu-id="349f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="349f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="349f1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="349f1-108">Permission type</span></span>      | <span data-ttu-id="349f1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="349f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="349f1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="349f1-110">Delegated (work or school account)</span></span>|<span data-ttu-id="349f1-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="349f1-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="349f1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="349f1-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="349f1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="349f1-113">Not supported.</span></span>|
|<span data-ttu-id="349f1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="349f1-114">Application</span></span>|<span data-ttu-id="349f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="349f1-115">Not supported.</span></span>|

<span data-ttu-id="349f1-116">Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="349f1-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="349f1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="349f1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="349f1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="349f1-118">Request headers</span></span>

|<span data-ttu-id="349f1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="349f1-119">Name</span></span>|<span data-ttu-id="349f1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="349f1-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="349f1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="349f1-121">Authorization</span></span>|<span data-ttu-id="349f1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="349f1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="349f1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="349f1-124">Content-Type</span></span>|<span data-ttu-id="349f1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="349f1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="349f1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="349f1-127">Request body</span></span>

<span data-ttu-id="349f1-128">В тексте запроса для представления JSON объекта [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="349f1-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="349f1-129">Требуются все свойства, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="349f1-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="349f1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="349f1-130">Property</span></span>|<span data-ttu-id="349f1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="349f1-131">Type</span></span>|<span data-ttu-id="349f1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="349f1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="349f1-133">clientId</span><span class="sxs-lookup"><span data-stu-id="349f1-133">clientId</span></span>|<span data-ttu-id="349f1-134">String</span><span class="sxs-lookup"><span data-stu-id="349f1-134">String</span></span>|<span data-ttu-id="349f1-135">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="349f1-135">The client ID for the application.</span></span> <span data-ttu-id="349f1-136">Это идентификатор клиента, полученные при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="349f1-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="349f1-137">client_secret</span><span class="sxs-lookup"><span data-stu-id="349f1-137">clientSecret</span></span>|<span data-ttu-id="349f1-138">String</span><span class="sxs-lookup"><span data-stu-id="349f1-138">String</span></span>|<span data-ttu-id="349f1-139">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="349f1-139">The client secret for the application.</span></span> <span data-ttu-id="349f1-140">Это секрет клиента, полученные при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="349f1-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="349f1-141">name</span><span class="sxs-lookup"><span data-stu-id="349f1-141">name</span></span>|<span data-ttu-id="349f1-142">String</span><span class="sxs-lookup"><span data-stu-id="349f1-142">String</span></span>|<span data-ttu-id="349f1-143">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="349f1-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="349f1-144">type</span><span class="sxs-lookup"><span data-stu-id="349f1-144">type</span></span>|<span data-ttu-id="349f1-145">String</span><span class="sxs-lookup"><span data-stu-id="349f1-145">String</span></span>|<span data-ttu-id="349f1-146">Тип поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="349f1-146">The identity provider type.</span></span> <span data-ttu-id="349f1-147">Оно должно быть одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="349f1-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="349f1-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="349f1-148">Microsoft</span></span><li/><span data-ttu-id="349f1-149">Google</span><span class="sxs-lookup"><span data-stu-id="349f1-149">Google</span></span><li/><span data-ttu-id="349f1-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="349f1-150">Amazon</span></span><li/><span data-ttu-id="349f1-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="349f1-151">LinkedIn</span></span><li/><span data-ttu-id="349f1-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="349f1-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="349f1-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="349f1-153">Response</span></span>

<span data-ttu-id="349f1-154">Успешно завершена, этот метод возвращает `201 Created` объект [identityProvider](../resources/identityprovider.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="349f1-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="349f1-155">В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="349f1-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="349f1-156">Пример</span><span class="sxs-lookup"><span data-stu-id="349f1-156">Example</span></span>

<span data-ttu-id="349f1-157">В следующем примере создается **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="349f1-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="349f1-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="349f1-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="349f1-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="349f1-159">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
