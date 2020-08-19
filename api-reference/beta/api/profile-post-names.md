---
title: Создание personName
description: Используйте этот API, чтобы создать новый personName в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ea4b8095d1af6e080e1e42162bbf1f8d56678446
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811639"
---
# <a name="create-personname"></a><span data-ttu-id="8ce9f-103">Создание personName</span><span class="sxs-lookup"><span data-stu-id="8ce9f-103">Create personName</span></span>

<span data-ttu-id="8ce9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ce9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ce9f-105">Используйте этот API, чтобы создать новый объект [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ce9f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ce9f-106">Permissions</span></span>

<span data-ttu-id="8ce9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ce9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ce9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ce9f-109">Permission type</span></span>                        | <span data-ttu-id="8ce9f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ce9f-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="8ce9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ce9f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ce9f-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8ce9f-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8ce9f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ce9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ce9f-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8ce9f-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8ce9f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ce9f-115">Application</span></span>                            | <span data-ttu-id="8ce9f-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8ce9f-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ce9f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ce9f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
POST /users/{id | userPrincipalName}/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="8ce9f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ce9f-118">Request headers</span></span>

| <span data-ttu-id="8ce9f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8ce9f-119">Name</span></span>           |<span data-ttu-id="8ce9f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8ce9f-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="8ce9f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ce9f-121">Authorization</span></span>  | <span data-ttu-id="8ce9f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8ce9f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ce9f-124">Content-Type</span></span>   | <span data-ttu-id="8ce9f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ce9f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ce9f-127">Request body</span></span>
<span data-ttu-id="8ce9f-128">В тексте запроса добавьте представление объекта [PersonName](../resources/personname.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-128">In the request body, supply a JSON representation of the [personName](../resources/personname.md) object.</span></span>

<span data-ttu-id="8ce9f-129">В следующей таблице приведены свойства, которые можно задать при создании объекта [PersonName](../resources/personname.md) .</span><span class="sxs-lookup"><span data-stu-id="8ce9f-129">The following table shows the properties that are possible to set when you create a [personName](../resources/personname.md) object.</span></span>

|<span data-ttu-id="8ce9f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ce9f-130">Property</span></span>|<span data-ttu-id="8ce9f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ce9f-131">Type</span></span>|<span data-ttu-id="8ce9f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ce9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ce9f-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="8ce9f-133">allowedAudiences</span></span>|<span data-ttu-id="8ce9f-134">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-134">String</span></span>|<span data-ttu-id="8ce9f-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8ce9f-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8ce9f-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8ce9f-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8ce9f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="8ce9f-138">displayName</span></span>|<span data-ttu-id="8ce9f-139">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-139">String</span></span>|<span data-ttu-id="8ce9f-140">Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-140">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span>|
|<span data-ttu-id="8ce9f-141">первыми</span><span class="sxs-lookup"><span data-stu-id="8ce9f-141">first</span></span>|<span data-ttu-id="8ce9f-142">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-142">String</span></span>|<span data-ttu-id="8ce9f-143">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-143">First name of the user.</span></span>|
|<span data-ttu-id="8ce9f-144">id</span><span class="sxs-lookup"><span data-stu-id="8ce9f-144">id</span></span>|<span data-ttu-id="8ce9f-145">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-145">String</span></span>|<span data-ttu-id="8ce9f-146">Идентификатор, используемый для индивидуальной адресации объекта.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-146">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="8ce9f-147">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="8ce9f-147">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="8ce9f-148">выводов</span><span class="sxs-lookup"><span data-stu-id="8ce9f-148">inference</span></span>|[<span data-ttu-id="8ce9f-149">инференцедата</span><span class="sxs-lookup"><span data-stu-id="8ce9f-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8ce9f-150">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8ce9f-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8ce9f-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8ce9f-152">initials</span><span class="sxs-lookup"><span data-stu-id="8ce9f-152">initials</span></span>|<span data-ttu-id="8ce9f-153">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-153">String</span></span>|<span data-ttu-id="8ce9f-154">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-154">Initials of the user.</span></span>|
|<span data-ttu-id="8ce9f-155">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="8ce9f-155">languageTag</span></span>|<span data-ttu-id="8ce9f-156">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-156">String</span></span>|<span data-ttu-id="8ce9f-157">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-157">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="8ce9f-158">Фамили</span><span class="sxs-lookup"><span data-stu-id="8ce9f-158">last</span></span>|<span data-ttu-id="8ce9f-159">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-159">String</span></span>|<span data-ttu-id="8ce9f-160">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-160">Last name of the user.</span></span>|
|<span data-ttu-id="8ce9f-161">маиден</span><span class="sxs-lookup"><span data-stu-id="8ce9f-161">maiden</span></span>|<span data-ttu-id="8ce9f-162">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-162">String</span></span>|<span data-ttu-id="8ce9f-163">Маиден имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-163">Maiden name of the user.</span></span> |
|<span data-ttu-id="8ce9f-164">назван</span><span class="sxs-lookup"><span data-stu-id="8ce9f-164">middle</span></span>|<span data-ttu-id="8ce9f-165">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-165">String</span></span>|<span data-ttu-id="8ce9f-166">Отчество пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-166">Middle name of the user.</span></span>|
|<span data-ttu-id="8ce9f-167">прозвищ</span><span class="sxs-lookup"><span data-stu-id="8ce9f-167">nickname</span></span>|<span data-ttu-id="8ce9f-168">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-168">String</span></span>|<span data-ttu-id="8ce9f-169">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-169">Nickname of the user.</span></span>|
|<span data-ttu-id="8ce9f-170">произношение</span><span class="sxs-lookup"><span data-stu-id="8ce9f-170">pronunciation</span></span>|[<span data-ttu-id="8ce9f-171">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="8ce9f-171">yomiPersonName</span></span>](../resources/yomipersonname.md)|<span data-ttu-id="8ce9f-172">Руководство по произношению имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-172">Guidance on how to pronounce the users name.</span></span>|
|<span data-ttu-id="8ce9f-173">суффикс</span><span class="sxs-lookup"><span data-stu-id="8ce9f-173">suffix</span></span>|<span data-ttu-id="8ce9f-174">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-174">String</span></span>|<span data-ttu-id="8ce9f-175">Обозначения, используемые после имени пользователя (например, "доктор").</span><span class="sxs-lookup"><span data-stu-id="8ce9f-175">Designators used after the users name (eg: PhD.)</span></span>  |
|<span data-ttu-id="8ce9f-176">title</span><span class="sxs-lookup"><span data-stu-id="8ce9f-176">title</span></span>|<span data-ttu-id="8ce9f-177">String</span><span class="sxs-lookup"><span data-stu-id="8ce9f-177">String</span></span>|<span data-ttu-id="8ce9f-178">Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).</span><span class="sxs-lookup"><span data-stu-id="8ce9f-178">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>|

## <a name="response"></a><span data-ttu-id="8ce9f-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ce9f-179">Response</span></span>

<span data-ttu-id="8ce9f-180">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-180">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ce9f-181">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ce9f-181">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ce9f-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ce9f-182">Request</span></span>

<span data-ttu-id="8ce9f-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ce9f-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ce9f-184">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="8ce9f-185">C#</span><span class="sxs-lookup"><span data-stu-id="8ce9f-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ce9f-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ce9f-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ce9f-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ce9f-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8ce9f-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ce9f-188">Response</span></span>

<span data-ttu-id="8ce9f-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-189">The following is an example of the response.</span></span>

> <span data-ttu-id="8ce9f-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ce9f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
