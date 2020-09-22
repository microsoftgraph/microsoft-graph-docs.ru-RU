---
title: Создание personName
description: Используйте этот API, чтобы создать новый personName в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e410904881c588dd2e15deef008fda089210335f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034478"
---
# <a name="create-personname"></a><span data-ttu-id="01b9e-103">Создание personName</span><span class="sxs-lookup"><span data-stu-id="01b9e-103">Create personName</span></span>

<span data-ttu-id="01b9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01b9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01b9e-105">Используйте этот API, чтобы создать новый объект [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="01b9e-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01b9e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01b9e-106">Permissions</span></span>

<span data-ttu-id="01b9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01b9e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01b9e-109">Permission type</span></span>                        | <span data-ttu-id="01b9e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01b9e-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="01b9e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01b9e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="01b9e-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="01b9e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="01b9e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01b9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01b9e-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="01b9e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="01b9e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01b9e-115">Application</span></span>                            | <span data-ttu-id="01b9e-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="01b9e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01b9e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01b9e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
POST /users/{id | userPrincipalName}/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="01b9e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01b9e-118">Request headers</span></span>

| <span data-ttu-id="01b9e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="01b9e-119">Name</span></span>           |<span data-ttu-id="01b9e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="01b9e-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="01b9e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01b9e-121">Authorization</span></span>  | <span data-ttu-id="01b9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01b9e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="01b9e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01b9e-124">Content-Type</span></span>   | <span data-ttu-id="01b9e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01b9e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01b9e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01b9e-127">Request body</span></span>
<span data-ttu-id="01b9e-128">В тексте запроса добавьте представление объекта [PersonName](../resources/personname.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01b9e-128">In the request body, supply a JSON representation of the [personName](../resources/personname.md) object.</span></span>

<span data-ttu-id="01b9e-129">В следующей таблице приведены свойства, которые можно задать при создании объекта [PersonName](../resources/personname.md) .</span><span class="sxs-lookup"><span data-stu-id="01b9e-129">The following table shows the properties that are possible to set when you create a [personName](../resources/personname.md) object.</span></span>

|<span data-ttu-id="01b9e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01b9e-130">Property</span></span>|<span data-ttu-id="01b9e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01b9e-131">Type</span></span>|<span data-ttu-id="01b9e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01b9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01b9e-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="01b9e-133">allowedAudiences</span></span>|<span data-ttu-id="01b9e-134">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-134">String</span></span>|<span data-ttu-id="01b9e-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="01b9e-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="01b9e-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="01b9e-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="01b9e-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="01b9e-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="01b9e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="01b9e-138">displayName</span></span>|<span data-ttu-id="01b9e-139">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-139">String</span></span>|<span data-ttu-id="01b9e-140">Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="01b9e-140">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="01b9e-141">первыми</span><span class="sxs-lookup"><span data-stu-id="01b9e-141">first</span></span>|<span data-ttu-id="01b9e-142">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-142">String</span></span>|<span data-ttu-id="01b9e-143">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="01b9e-143">First name of the user.</span></span>|
|<span data-ttu-id="01b9e-144">id</span><span class="sxs-lookup"><span data-stu-id="01b9e-144">id</span></span>|<span data-ttu-id="01b9e-145">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-145">String</span></span>|<span data-ttu-id="01b9e-146">Идентификатор, используемый для индивидуальной адресации объекта.</span><span class="sxs-lookup"><span data-stu-id="01b9e-146">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="01b9e-147">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="01b9e-147">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="01b9e-148">выводов</span><span class="sxs-lookup"><span data-stu-id="01b9e-148">inference</span></span>|[<span data-ttu-id="01b9e-149">инференцедата</span><span class="sxs-lookup"><span data-stu-id="01b9e-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="01b9e-150">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="01b9e-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="01b9e-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="01b9e-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="01b9e-152">initials</span><span class="sxs-lookup"><span data-stu-id="01b9e-152">initials</span></span>|<span data-ttu-id="01b9e-153">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-153">String</span></span>|<span data-ttu-id="01b9e-154">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="01b9e-154">Initials of the user.</span></span>|
|<span data-ttu-id="01b9e-155">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="01b9e-155">languageTag</span></span>|<span data-ttu-id="01b9e-156">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-156">String</span></span>|<span data-ttu-id="01b9e-157">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="01b9e-157">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="01b9e-158">Фамили</span><span class="sxs-lookup"><span data-stu-id="01b9e-158">last</span></span>|<span data-ttu-id="01b9e-159">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-159">String</span></span>|<span data-ttu-id="01b9e-160">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="01b9e-160">Last name of the user.</span></span>|
|<span data-ttu-id="01b9e-161">маиден</span><span class="sxs-lookup"><span data-stu-id="01b9e-161">maiden</span></span>|<span data-ttu-id="01b9e-162">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-162">String</span></span>|<span data-ttu-id="01b9e-163">Маиден имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="01b9e-163">Maiden name of the user.</span></span> |
|<span data-ttu-id="01b9e-164">назван</span><span class="sxs-lookup"><span data-stu-id="01b9e-164">middle</span></span>|<span data-ttu-id="01b9e-165">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-165">String</span></span>|<span data-ttu-id="01b9e-166">Отчество пользователя.</span><span class="sxs-lookup"><span data-stu-id="01b9e-166">Middle name of the user.</span></span>|
|<span data-ttu-id="01b9e-167">прозвищ</span><span class="sxs-lookup"><span data-stu-id="01b9e-167">nickname</span></span>|<span data-ttu-id="01b9e-168">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-168">String</span></span>|<span data-ttu-id="01b9e-169">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="01b9e-169">Nickname of the user.</span></span>|
|<span data-ttu-id="01b9e-170">произношение</span><span class="sxs-lookup"><span data-stu-id="01b9e-170">pronunciation</span></span>|[<span data-ttu-id="01b9e-171">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="01b9e-171">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="01b9e-172">Руководство по произношению имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="01b9e-172">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="01b9e-173">суффикс</span><span class="sxs-lookup"><span data-stu-id="01b9e-173">suffix</span></span>|<span data-ttu-id="01b9e-174">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-174">String</span></span>|<span data-ttu-id="01b9e-175">Обозначения, используемые после имени пользователя (например, "доктор").</span><span class="sxs-lookup"><span data-stu-id="01b9e-175">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="01b9e-176">title</span><span class="sxs-lookup"><span data-stu-id="01b9e-176">title</span></span>|<span data-ttu-id="01b9e-177">String</span><span class="sxs-lookup"><span data-stu-id="01b9e-177">String</span></span>|<span data-ttu-id="01b9e-178">Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).</span><span class="sxs-lookup"><span data-stu-id="01b9e-178">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="01b9e-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="01b9e-179">Response</span></span>

<span data-ttu-id="01b9e-180">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01b9e-180">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01b9e-181">Примеры</span><span class="sxs-lookup"><span data-stu-id="01b9e-181">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01b9e-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="01b9e-182">Request</span></span>

<span data-ttu-id="01b9e-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01b9e-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01b9e-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="01b9e-184">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="01b9e-185">C#</span><span class="sxs-lookup"><span data-stu-id="01b9e-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01b9e-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01b9e-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01b9e-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01b9e-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="01b9e-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="01b9e-188">Response</span></span>

<span data-ttu-id="01b9e-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01b9e-189">The following is an example of the response.</span></span>

> <span data-ttu-id="01b9e-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01b9e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


