---
title: Обновление personName
description: Обновление свойств объекта personName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 540ce931e77b5f9347015fe5792c7c2e0f5486f8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972739"
---
# <a name="update-personname"></a><span data-ttu-id="7dd0c-103">Обновление PersonName</span><span class="sxs-lookup"><span data-stu-id="7dd0c-103">Update personname</span></span>

<span data-ttu-id="7dd0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dd0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dd0c-105">Обновление свойств объекта [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7dd0c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dd0c-106">Permissions</span></span>

<span data-ttu-id="7dd0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dd0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7dd0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dd0c-109">Permission type</span></span>                        | <span data-ttu-id="7dd0c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dd0c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7dd0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dd0c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7dd0c-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7dd0c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7dd0c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dd0c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dd0c-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7dd0c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7dd0c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dd0c-115">Application</span></span>                            | <span data-ttu-id="7dd0c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dd0c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="7dd0c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dd0c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
PATCH /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7dd0c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dd0c-118">Request headers</span></span>

| <span data-ttu-id="7dd0c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7dd0c-119">Name</span></span>           |<span data-ttu-id="7dd0c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd0c-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="7dd0c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dd0c-121">Authorization</span></span>  | <span data-ttu-id="7dd0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7dd0c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7dd0c-124">Content-Type</span></span>   | <span data-ttu-id="7dd0c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dd0c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7dd0c-127">Request body</span></span>

<span data-ttu-id="7dd0c-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7dd0c-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7dd0c-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="7dd0c-131">В следующей таблице приведены свойства, которые можно обновлять в существующем объекте [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-131">The following table shows the properties that are possible to update within an existing [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="7dd0c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dd0c-132">Property</span></span>|<span data-ttu-id="7dd0c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="7dd0c-133">Type</span></span>|<span data-ttu-id="7dd0c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd0c-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dd0c-135">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="7dd0c-135">allowedAudiences</span></span>|<span data-ttu-id="7dd0c-136">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-136">String</span></span>|<span data-ttu-id="7dd0c-137">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="7dd0c-138">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="7dd0c-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="7dd0c-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7dd0c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7dd0c-140">displayName</span></span>|<span data-ttu-id="7dd0c-141">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-141">String</span></span>|<span data-ttu-id="7dd0c-142">Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-142">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="7dd0c-143">первыми</span><span class="sxs-lookup"><span data-stu-id="7dd0c-143">first</span></span>|<span data-ttu-id="7dd0c-144">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-144">String</span></span>|<span data-ttu-id="7dd0c-145">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-145">First name of the user.</span></span>|
|<span data-ttu-id="7dd0c-146">выводов</span><span class="sxs-lookup"><span data-stu-id="7dd0c-146">inference</span></span>|[<span data-ttu-id="7dd0c-147">инференцедата</span><span class="sxs-lookup"><span data-stu-id="7dd0c-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="7dd0c-148">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="7dd0c-149">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="7dd0c-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="7dd0c-150">initials</span><span class="sxs-lookup"><span data-stu-id="7dd0c-150">initials</span></span>|<span data-ttu-id="7dd0c-151">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-151">String</span></span>|<span data-ttu-id="7dd0c-152">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-152">Initials of the user.</span></span>|
|<span data-ttu-id="7dd0c-153">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="7dd0c-153">languageTag</span></span>|<span data-ttu-id="7dd0c-154">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-154">String</span></span>|<span data-ttu-id="7dd0c-155">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-155">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="7dd0c-156">Фамили</span><span class="sxs-lookup"><span data-stu-id="7dd0c-156">last</span></span>|<span data-ttu-id="7dd0c-157">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-157">String</span></span>|<span data-ttu-id="7dd0c-158">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-158">Last name of the user.</span></span>|
|<span data-ttu-id="7dd0c-159">маиден</span><span class="sxs-lookup"><span data-stu-id="7dd0c-159">maiden</span></span>|<span data-ttu-id="7dd0c-160">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-160">String</span></span>|<span data-ttu-id="7dd0c-161">Маиден имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-161">Maiden name of the user.</span></span> |
|<span data-ttu-id="7dd0c-162">назван</span><span class="sxs-lookup"><span data-stu-id="7dd0c-162">middle</span></span>|<span data-ttu-id="7dd0c-163">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-163">String</span></span>|<span data-ttu-id="7dd0c-164">Отчество пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-164">Middle name of the user.</span></span>|
|<span data-ttu-id="7dd0c-165">прозвищ</span><span class="sxs-lookup"><span data-stu-id="7dd0c-165">nickname</span></span>|<span data-ttu-id="7dd0c-166">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-166">String</span></span>|<span data-ttu-id="7dd0c-167">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-167">Nickname of the user.</span></span>|
|<span data-ttu-id="7dd0c-168">произношение</span><span class="sxs-lookup"><span data-stu-id="7dd0c-168">pronunciation</span></span>|[<span data-ttu-id="7dd0c-169">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="7dd0c-169">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="7dd0c-170">Руководство по произношению имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-170">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="7dd0c-171">суффикс</span><span class="sxs-lookup"><span data-stu-id="7dd0c-171">suffix</span></span>|<span data-ttu-id="7dd0c-172">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-172">String</span></span>|<span data-ttu-id="7dd0c-173">Обозначения, используемые после имени пользователя (например, "доктор").</span><span class="sxs-lookup"><span data-stu-id="7dd0c-173">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="7dd0c-174">title</span><span class="sxs-lookup"><span data-stu-id="7dd0c-174">title</span></span>|<span data-ttu-id="7dd0c-175">String</span><span class="sxs-lookup"><span data-stu-id="7dd0c-175">String</span></span>|<span data-ttu-id="7dd0c-176">Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).</span><span class="sxs-lookup"><span data-stu-id="7dd0c-176">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="7dd0c-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd0c-177">Response</span></span>

<span data-ttu-id="7dd0c-178">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-178">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7dd0c-179">Примеры</span><span class="sxs-lookup"><span data-stu-id="7dd0c-179">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7dd0c-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dd0c-180">Request</span></span>

<span data-ttu-id="7dd0c-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-181">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7dd0c-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dd0c-182">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7dd0c-183">C#</span><span class="sxs-lookup"><span data-stu-id="7dd0c-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dd0c-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dd0c-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dd0c-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dd0c-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dd0c-186">Java</span><span class="sxs-lookup"><span data-stu-id="7dd0c-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personname-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7dd0c-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd0c-187">Response</span></span>

<span data-ttu-id="7dd0c-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-188">The following is an example of the response.</span></span>

> <span data-ttu-id="7dd0c-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dd0c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


