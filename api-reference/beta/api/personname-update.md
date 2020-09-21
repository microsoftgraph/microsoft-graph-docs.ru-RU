---
title: Обновление personName
description: Обновление свойств объекта personName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 015ac0a0829964fb54f306375d00470ea89ab2ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969314"
---
# <a name="update-personname"></a><span data-ttu-id="b0f85-103">Обновление PersonName</span><span class="sxs-lookup"><span data-stu-id="b0f85-103">Update personname</span></span>

<span data-ttu-id="b0f85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0f85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0f85-105">Обновление свойств объекта [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0f85-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0f85-106">Permissions</span></span>

<span data-ttu-id="b0f85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0f85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0f85-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0f85-109">Permission type</span></span>                        | <span data-ttu-id="b0f85-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0f85-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b0f85-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0f85-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0f85-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b0f85-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b0f85-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0f85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0f85-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b0f85-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b0f85-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0f85-115">Application</span></span>                            | <span data-ttu-id="b0f85-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0f85-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="b0f85-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0f85-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
PATCH /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b0f85-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0f85-118">Request headers</span></span>

| <span data-ttu-id="b0f85-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b0f85-119">Name</span></span>           |<span data-ttu-id="b0f85-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b0f85-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b0f85-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0f85-121">Authorization</span></span>  | <span data-ttu-id="b0f85-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0f85-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b0f85-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0f85-124">Content-Type</span></span>   | <span data-ttu-id="b0f85-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0f85-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0f85-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0f85-127">Request body</span></span>

<span data-ttu-id="b0f85-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b0f85-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b0f85-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b0f85-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b0f85-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b0f85-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="b0f85-131">В следующей таблице приведены свойства, которые можно обновлять в существующем объекте [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-131">The following table shows the properties that are possible to update within an existing [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="b0f85-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0f85-132">Property</span></span>|<span data-ttu-id="b0f85-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b0f85-133">Type</span></span>|<span data-ttu-id="b0f85-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b0f85-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0f85-135">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="b0f85-135">allowedAudiences</span></span>|<span data-ttu-id="b0f85-136">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-136">String</span></span>|<span data-ttu-id="b0f85-137">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="b0f85-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="b0f85-138">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b0f85-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="b0f85-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b0f85-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b0f85-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b0f85-140">displayName</span></span>|<span data-ttu-id="b0f85-141">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-141">String</span></span>|<span data-ttu-id="b0f85-142">Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="b0f85-142">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="b0f85-143">первыми</span><span class="sxs-lookup"><span data-stu-id="b0f85-143">first</span></span>|<span data-ttu-id="b0f85-144">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-144">String</span></span>|<span data-ttu-id="b0f85-145">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-145">First name of the user.</span></span>|
|<span data-ttu-id="b0f85-146">выводов</span><span class="sxs-lookup"><span data-stu-id="b0f85-146">inference</span></span>|[<span data-ttu-id="b0f85-147">инференцедата</span><span class="sxs-lookup"><span data-stu-id="b0f85-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="b0f85-148">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="b0f85-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="b0f85-149">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b0f85-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="b0f85-150">initials</span><span class="sxs-lookup"><span data-stu-id="b0f85-150">initials</span></span>|<span data-ttu-id="b0f85-151">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-151">String</span></span>|<span data-ttu-id="b0f85-152">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-152">Initials of the user.</span></span>|
|<span data-ttu-id="b0f85-153">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="b0f85-153">languageTag</span></span>|<span data-ttu-id="b0f85-154">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-154">String</span></span>|<span data-ttu-id="b0f85-155">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="b0f85-155">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="b0f85-156">Фамили</span><span class="sxs-lookup"><span data-stu-id="b0f85-156">last</span></span>|<span data-ttu-id="b0f85-157">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-157">String</span></span>|<span data-ttu-id="b0f85-158">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-158">Last name of the user.</span></span>|
|<span data-ttu-id="b0f85-159">маиден</span><span class="sxs-lookup"><span data-stu-id="b0f85-159">maiden</span></span>|<span data-ttu-id="b0f85-160">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-160">String</span></span>|<span data-ttu-id="b0f85-161">Маиден имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-161">Maiden name of the user.</span></span> |
|<span data-ttu-id="b0f85-162">назван</span><span class="sxs-lookup"><span data-stu-id="b0f85-162">middle</span></span>|<span data-ttu-id="b0f85-163">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-163">String</span></span>|<span data-ttu-id="b0f85-164">Отчество пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-164">Middle name of the user.</span></span>|
|<span data-ttu-id="b0f85-165">прозвищ</span><span class="sxs-lookup"><span data-stu-id="b0f85-165">nickname</span></span>|<span data-ttu-id="b0f85-166">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-166">String</span></span>|<span data-ttu-id="b0f85-167">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-167">Nickname of the user.</span></span>|
|<span data-ttu-id="b0f85-168">произношение</span><span class="sxs-lookup"><span data-stu-id="b0f85-168">pronunciation</span></span>|[<span data-ttu-id="b0f85-169">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="b0f85-169">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="b0f85-170">Руководство по произношению имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0f85-170">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="b0f85-171">суффикс</span><span class="sxs-lookup"><span data-stu-id="b0f85-171">suffix</span></span>|<span data-ttu-id="b0f85-172">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-172">String</span></span>|<span data-ttu-id="b0f85-173">Обозначения, используемые после имени пользователя (например, "доктор").</span><span class="sxs-lookup"><span data-stu-id="b0f85-173">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="b0f85-174">title</span><span class="sxs-lookup"><span data-stu-id="b0f85-174">title</span></span>|<span data-ttu-id="b0f85-175">String</span><span class="sxs-lookup"><span data-stu-id="b0f85-175">String</span></span>|<span data-ttu-id="b0f85-176">Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).</span><span class="sxs-lookup"><span data-stu-id="b0f85-176">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="b0f85-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0f85-177">Response</span></span>

<span data-ttu-id="b0f85-178">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0f85-178">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0f85-179">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0f85-179">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0f85-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0f85-180">Request</span></span>

<span data-ttu-id="b0f85-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0f85-181">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0f85-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0f85-182">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b0f85-183">C#</span><span class="sxs-lookup"><span data-stu-id="b0f85-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0f85-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0f85-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0f85-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0f85-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b0f85-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0f85-186">Response</span></span>

<span data-ttu-id="b0f85-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b0f85-187">The following is an example of the response.</span></span>

> <span data-ttu-id="b0f85-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0f85-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


