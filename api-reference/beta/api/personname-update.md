---
title: Обновление personName
description: Обновление свойств объекта personName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0959c7eec1b1e52ff3a9295ad7e5af07b416a3bd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051104"
---
# <a name="update-personname"></a><span data-ttu-id="e065f-103">Обновление имени пользователя</span><span class="sxs-lookup"><span data-stu-id="e065f-103">Update personname</span></span>

<span data-ttu-id="e065f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e065f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e065f-105">Обновление свойств объекта [personName](../resources/personname.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="e065f-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e065f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e065f-106">Permissions</span></span>

<span data-ttu-id="e065f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e065f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e065f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e065f-109">Permission type</span></span>                        | <span data-ttu-id="e065f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e065f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e065f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e065f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e065f-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e065f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e065f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e065f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e065f-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e065f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e065f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e065f-115">Application</span></span>                            | <span data-ttu-id="e065f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e065f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e065f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e065f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
PATCH /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e065f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e065f-118">Request headers</span></span>

| <span data-ttu-id="e065f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e065f-119">Name</span></span>           |<span data-ttu-id="e065f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e065f-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e065f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e065f-121">Authorization</span></span>  | <span data-ttu-id="e065f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e065f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e065f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e065f-124">Content-Type</span></span>   | <span data-ttu-id="e065f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e065f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e065f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e065f-127">Request body</span></span>

<span data-ttu-id="e065f-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e065f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e065f-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e065f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e065f-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e065f-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="e065f-131">В следующей таблице показаны свойства, которые можно обновить в существующем объекте [personName](../resources/personname.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="e065f-131">The following table shows the properties that are possible to update within an existing [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="e065f-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="e065f-132">Property</span></span>|<span data-ttu-id="e065f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e065f-133">Type</span></span>|<span data-ttu-id="e065f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e065f-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e065f-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="e065f-135">allowedAudiences</span></span>|<span data-ttu-id="e065f-136">String</span><span class="sxs-lookup"><span data-stu-id="e065f-136">String</span></span>|<span data-ttu-id="e065f-137">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="e065f-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e065f-138">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e065f-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e065f-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e065f-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e065f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="e065f-140">displayName</span></span>|<span data-ttu-id="e065f-141">String</span><span class="sxs-lookup"><span data-stu-id="e065f-141">String</span></span>|<span data-ttu-id="e065f-142">Предоставляет упорядоченную отрисовку firstName и lastName в зависимости от локализа пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="e065f-142">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="e065f-143">во-первых</span><span class="sxs-lookup"><span data-stu-id="e065f-143">first</span></span>|<span data-ttu-id="e065f-144">String</span><span class="sxs-lookup"><span data-stu-id="e065f-144">String</span></span>|<span data-ttu-id="e065f-145">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e065f-145">First name of the user.</span></span>|
|<span data-ttu-id="e065f-146">вывод</span><span class="sxs-lookup"><span data-stu-id="e065f-146">inference</span></span>|[<span data-ttu-id="e065f-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="e065f-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e065f-148">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="e065f-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e065f-149">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e065f-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e065f-150">initials</span><span class="sxs-lookup"><span data-stu-id="e065f-150">initials</span></span>|<span data-ttu-id="e065f-151">String</span><span class="sxs-lookup"><span data-stu-id="e065f-151">String</span></span>|<span data-ttu-id="e065f-152">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="e065f-152">Initials of the user.</span></span>|
|<span data-ttu-id="e065f-153">LanguageTag</span><span class="sxs-lookup"><span data-stu-id="e065f-153">languageTag</span></span>|<span data-ttu-id="e065f-154">String</span><span class="sxs-lookup"><span data-stu-id="e065f-154">String</span></span>|<span data-ttu-id="e065f-155">Содержит имя языка (en-US, no-NB, ru-AU) в формате IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="e065f-155">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="e065f-156">последний</span><span class="sxs-lookup"><span data-stu-id="e065f-156">last</span></span>|<span data-ttu-id="e065f-157">String</span><span class="sxs-lookup"><span data-stu-id="e065f-157">String</span></span>|<span data-ttu-id="e065f-158">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="e065f-158">Last name of the user.</span></span>|
|<span data-ttu-id="e065f-159">maiden</span><span class="sxs-lookup"><span data-stu-id="e065f-159">maiden</span></span>|<span data-ttu-id="e065f-160">String</span><span class="sxs-lookup"><span data-stu-id="e065f-160">String</span></span>|<span data-ttu-id="e065f-161">Девичья фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="e065f-161">Maiden name of the user.</span></span> |
|<span data-ttu-id="e065f-162">средний</span><span class="sxs-lookup"><span data-stu-id="e065f-162">middle</span></span>|<span data-ttu-id="e065f-163">String</span><span class="sxs-lookup"><span data-stu-id="e065f-163">String</span></span>|<span data-ttu-id="e065f-164">Среднее имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e065f-164">Middle name of the user.</span></span>|
|<span data-ttu-id="e065f-165">nickname</span><span class="sxs-lookup"><span data-stu-id="e065f-165">nickname</span></span>|<span data-ttu-id="e065f-166">String</span><span class="sxs-lookup"><span data-stu-id="e065f-166">String</span></span>|<span data-ttu-id="e065f-167">Прозвище пользователя.</span><span class="sxs-lookup"><span data-stu-id="e065f-167">Nickname of the user.</span></span>|
|<span data-ttu-id="e065f-168">произношение</span><span class="sxs-lookup"><span data-stu-id="e065f-168">pronunciation</span></span>|[<span data-ttu-id="e065f-169">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="e065f-169">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="e065f-170">Руководство по произносить имя пользователей.</span><span class="sxs-lookup"><span data-stu-id="e065f-170">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="e065f-171">суффикс</span><span class="sxs-lookup"><span data-stu-id="e065f-171">suffix</span></span>|<span data-ttu-id="e065f-172">String</span><span class="sxs-lookup"><span data-stu-id="e065f-172">String</span></span>|<span data-ttu-id="e065f-173">Назначенные элементы, используемые после имени пользователей (например: PhD.)</span><span class="sxs-lookup"><span data-stu-id="e065f-173">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="e065f-174">title</span><span class="sxs-lookup"><span data-stu-id="e065f-174">title</span></span>|<span data-ttu-id="e065f-175">String</span><span class="sxs-lookup"><span data-stu-id="e065f-175">String</span></span>|<span data-ttu-id="e065f-176">Honorifics used to prefix a users name (eg: Dr, Sir, Msam, Mrs.)</span><span class="sxs-lookup"><span data-stu-id="e065f-176">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="e065f-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="e065f-177">Response</span></span>

<span data-ttu-id="e065f-178">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [personName](../resources/personname.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e065f-178">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e065f-179">Примеры</span><span class="sxs-lookup"><span data-stu-id="e065f-179">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e065f-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="e065f-180">Request</span></span>

<span data-ttu-id="e065f-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e065f-181">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e065f-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="e065f-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personname"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/names/{id}
Content-type: application/json

{
  "nickname": "Kesha"
}

```
# <a name="c"></a>[<span data-ttu-id="e065f-183">C#</span><span class="sxs-lookup"><span data-stu-id="e065f-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e065f-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e065f-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e065f-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e065f-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e065f-186">Java</span><span class="sxs-lookup"><span data-stu-id="e065f-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personname-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e065f-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="e065f-187">Response</span></span>

<span data-ttu-id="e065f-188">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e065f-188">The following is an example of the response.</span></span>

> <span data-ttu-id="e065f-189">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e065f-189">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 200 OK
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
  "nickname": "Kesha",
  "suffix": null,
  "title": null,
  "pronunciation": {
    "displayName": "In-no ken-te ",
    "first": "In-no ken-te Pop-ov",
    "maiden": null,
    "middle": null,
    "last": "Pop-ov"
  }
}
```


