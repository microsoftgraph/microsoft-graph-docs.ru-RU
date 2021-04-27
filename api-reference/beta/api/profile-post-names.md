---
title: Создание personName
description: Используйте этот API, чтобы создать новое имя пользователя в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f29c138fbf2a0dfe374111bfa6f9d2511f5e62b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036886"
---
# <a name="create-personname"></a><span data-ttu-id="5e71c-103">Создание personName</span><span class="sxs-lookup"><span data-stu-id="5e71c-103">Create personName</span></span>

<span data-ttu-id="5e71c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e71c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e71c-105">Используйте этот API для создания нового [объекта personName](../resources/personname.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="5e71c-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e71c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e71c-106">Permissions</span></span>

<span data-ttu-id="5e71c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e71c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e71c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e71c-109">Permission type</span></span>                        | <span data-ttu-id="5e71c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e71c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="5e71c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e71c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e71c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e71c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5e71c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e71c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e71c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e71c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5e71c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e71c-115">Application</span></span>                            | <span data-ttu-id="5e71c-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e71c-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e71c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e71c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
POST /users/{id | userPrincipalName}/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="5e71c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e71c-118">Request headers</span></span>

| <span data-ttu-id="5e71c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5e71c-119">Name</span></span>           |<span data-ttu-id="5e71c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5e71c-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="5e71c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e71c-121">Authorization</span></span>  | <span data-ttu-id="5e71c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e71c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5e71c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e71c-124">Content-Type</span></span>   | <span data-ttu-id="5e71c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e71c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e71c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e71c-127">Request body</span></span>
<span data-ttu-id="5e71c-128">В теле запроса поставляем представление JSON объекта [personName.](../resources/personname.md)</span><span class="sxs-lookup"><span data-stu-id="5e71c-128">In the request body, supply a JSON representation of the [personName](../resources/personname.md) object.</span></span>

<span data-ttu-id="5e71c-129">В следующей таблице показаны свойства, которые можно установить при создании [объекта personName.](../resources/personname.md)</span><span class="sxs-lookup"><span data-stu-id="5e71c-129">The following table shows the properties that are possible to set when you create a [personName](../resources/personname.md) object.</span></span>

|<span data-ttu-id="5e71c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e71c-130">Property</span></span>|<span data-ttu-id="5e71c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5e71c-131">Type</span></span>|<span data-ttu-id="5e71c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5e71c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e71c-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="5e71c-133">allowedAudiences</span></span>|<span data-ttu-id="5e71c-134">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-134">String</span></span>|<span data-ttu-id="5e71c-135">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="5e71c-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="5e71c-136">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e71c-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="5e71c-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5e71c-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5e71c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5e71c-138">displayName</span></span>|<span data-ttu-id="5e71c-139">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-139">String</span></span>|<span data-ttu-id="5e71c-140">Предоставляет упорядоченную отрисовку firstName и lastName в зависимости от локализа пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="5e71c-140">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="5e71c-141">во-первых</span><span class="sxs-lookup"><span data-stu-id="5e71c-141">first</span></span>|<span data-ttu-id="5e71c-142">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-142">String</span></span>|<span data-ttu-id="5e71c-143">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e71c-143">First name of the user.</span></span>|
|<span data-ttu-id="5e71c-144">id</span><span class="sxs-lookup"><span data-stu-id="5e71c-144">id</span></span>|<span data-ttu-id="5e71c-145">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-145">String</span></span>|<span data-ttu-id="5e71c-146">Идентификатор, используемый для индивидуального обращения к объекту.</span><span class="sxs-lookup"><span data-stu-id="5e71c-146">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="5e71c-147">Унаследованный от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="5e71c-147">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="5e71c-148">вывод</span><span class="sxs-lookup"><span data-stu-id="5e71c-148">inference</span></span>|[<span data-ttu-id="5e71c-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="5e71c-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="5e71c-150">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="5e71c-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="5e71c-151">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5e71c-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5e71c-152">initials</span><span class="sxs-lookup"><span data-stu-id="5e71c-152">initials</span></span>|<span data-ttu-id="5e71c-153">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-153">String</span></span>|<span data-ttu-id="5e71c-154">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e71c-154">Initials of the user.</span></span>|
|<span data-ttu-id="5e71c-155">LanguageTag</span><span class="sxs-lookup"><span data-stu-id="5e71c-155">languageTag</span></span>|<span data-ttu-id="5e71c-156">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-156">String</span></span>|<span data-ttu-id="5e71c-157">Содержит имя языка (en-US, no-NB, ru-AU) в формате IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="5e71c-157">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="5e71c-158">последний</span><span class="sxs-lookup"><span data-stu-id="5e71c-158">last</span></span>|<span data-ttu-id="5e71c-159">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-159">String</span></span>|<span data-ttu-id="5e71c-160">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e71c-160">Last name of the user.</span></span>|
|<span data-ttu-id="5e71c-161">maiden</span><span class="sxs-lookup"><span data-stu-id="5e71c-161">maiden</span></span>|<span data-ttu-id="5e71c-162">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-162">String</span></span>|<span data-ttu-id="5e71c-163">Девичья фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e71c-163">Maiden name of the user.</span></span> |
|<span data-ttu-id="5e71c-164">средний</span><span class="sxs-lookup"><span data-stu-id="5e71c-164">middle</span></span>|<span data-ttu-id="5e71c-165">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-165">String</span></span>|<span data-ttu-id="5e71c-166">Среднее имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e71c-166">Middle name of the user.</span></span>|
|<span data-ttu-id="5e71c-167">nickname</span><span class="sxs-lookup"><span data-stu-id="5e71c-167">nickname</span></span>|<span data-ttu-id="5e71c-168">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-168">String</span></span>|<span data-ttu-id="5e71c-169">Прозвище пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e71c-169">Nickname of the user.</span></span>|
|<span data-ttu-id="5e71c-170">произношение</span><span class="sxs-lookup"><span data-stu-id="5e71c-170">pronunciation</span></span>|[<span data-ttu-id="5e71c-171">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="5e71c-171">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="5e71c-172">Руководство по произносить имя пользователей.</span><span class="sxs-lookup"><span data-stu-id="5e71c-172">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="5e71c-173">суффикс</span><span class="sxs-lookup"><span data-stu-id="5e71c-173">suffix</span></span>|<span data-ttu-id="5e71c-174">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-174">String</span></span>|<span data-ttu-id="5e71c-175">Назначенные элементы, используемые после имени пользователей (например: PhD.)</span><span class="sxs-lookup"><span data-stu-id="5e71c-175">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="5e71c-176">title</span><span class="sxs-lookup"><span data-stu-id="5e71c-176">title</span></span>|<span data-ttu-id="5e71c-177">String</span><span class="sxs-lookup"><span data-stu-id="5e71c-177">String</span></span>|<span data-ttu-id="5e71c-178">Honorifics used to prefix a users name (eg: Dr, Sir, Msam, Mrs.)</span><span class="sxs-lookup"><span data-stu-id="5e71c-178">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="5e71c-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e71c-179">Response</span></span>

<span data-ttu-id="5e71c-180">В случае успешной работы этот метод возвращает код ответа и `201, Created` новый [объект personName](../resources/personname.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5e71c-180">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e71c-181">Примеры</span><span class="sxs-lookup"><span data-stu-id="5e71c-181">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e71c-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e71c-182">Request</span></span>

<span data-ttu-id="5e71c-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e71c-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e71c-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e71c-184">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null
}
```
# <a name="c"></a>[<span data-ttu-id="5e71c-185">C#</span><span class="sxs-lookup"><span data-stu-id="5e71c-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e71c-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e71c-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e71c-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e71c-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e71c-188">Java</span><span class="sxs-lookup"><span data-stu-id="5e71c-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personname-from-profilev2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5e71c-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e71c-189">Response</span></span>

<span data-ttu-id="5e71c-190">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5e71c-190">The following is an example of the response.</span></span>

> <span data-ttu-id="5e71c-191">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5e71c-191">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": null,
  "suffix": null,
  "title": null,
  "pronunciation": null
}
```


