---
title: Обновление personName
description: Обновление свойств объекта PersonName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f288d73956b79c0ab5c47524239069f2c239791c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997224"
---
# <a name="update-personname"></a><span data-ttu-id="2d29d-103">Обновление PersonName</span><span class="sxs-lookup"><span data-stu-id="2d29d-103">Update personname</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d29d-104">Обновление свойств объекта [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-104">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d29d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d29d-105">Permissions</span></span>

<span data-ttu-id="2d29d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d29d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d29d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d29d-108">Permission type</span></span>                        | <span data-ttu-id="2d29d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d29d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2d29d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d29d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d29d-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2d29d-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2d29d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d29d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d29d-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2d29d-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2d29d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d29d-114">Application</span></span>                            | <span data-ttu-id="2d29d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d29d-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="2d29d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d29d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2d29d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d29d-117">Request headers</span></span>

| <span data-ttu-id="2d29d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2d29d-118">Name</span></span>           |<span data-ttu-id="2d29d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2d29d-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="2d29d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d29d-120">Authorization</span></span>  | <span data-ttu-id="2d29d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d29d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2d29d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d29d-123">Content-Type</span></span>   | <span data-ttu-id="2d29d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d29d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d29d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d29d-126">Request body</span></span>

<span data-ttu-id="2d29d-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2d29d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2d29d-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="2d29d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2d29d-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2d29d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2d29d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d29d-130">Property</span></span>     | <span data-ttu-id="2d29d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2d29d-131">Type</span></span>                                            | <span data-ttu-id="2d29d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2d29d-132">Description</span></span>                                                                             | 
|:-------------|:------------------------------------------------|:----------------------------------------------------------------------------------------|
|<span data-ttu-id="2d29d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2d29d-133">displayName</span></span>   |<span data-ttu-id="2d29d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2d29d-134">String</span></span>                                           | <span data-ttu-id="2d29d-135">Предоставляет упорядоченную визуализацию имени и фамилии.</span><span class="sxs-lookup"><span data-stu-id="2d29d-135">Provides an ordered rendering of first name and last name.</span></span>                              |
|<span data-ttu-id="2d29d-136">первыми</span><span class="sxs-lookup"><span data-stu-id="2d29d-136">first</span></span>         |<span data-ttu-id="2d29d-137">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-137">String</span></span>                                           | <span data-ttu-id="2d29d-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-138">First Name of the user.</span></span>                                                                 |
|<span data-ttu-id="2d29d-139">initials</span><span class="sxs-lookup"><span data-stu-id="2d29d-139">initials</span></span>      |<span data-ttu-id="2d29d-140">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-140">String</span></span>                                           | <span data-ttu-id="2d29d-141">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-141">Initials of the user.</span></span>                                                                   |
|<span data-ttu-id="2d29d-142">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="2d29d-142">languageTag</span></span>   |<span data-ttu-id="2d29d-143">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-143">String</span></span>                                           | <span data-ttu-id="2d29d-144">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="2d29d-144">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="2d29d-145">Фамили</span><span class="sxs-lookup"><span data-stu-id="2d29d-145">last</span></span>          |<span data-ttu-id="2d29d-146">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-146">String</span></span>                                           | <span data-ttu-id="2d29d-147">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-147">Last name of the user.</span></span>                                                                  |
|<span data-ttu-id="2d29d-148">маиден</span><span class="sxs-lookup"><span data-stu-id="2d29d-148">maiden</span></span>        |<span data-ttu-id="2d29d-149">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-149">String</span></span>                                           | <span data-ttu-id="2d29d-150">Имя пользователя, марриаже фамилию.</span><span class="sxs-lookup"><span data-stu-id="2d29d-150">User's pre-marriage last name.</span></span>                                                          |
|<span data-ttu-id="2d29d-151">назван</span><span class="sxs-lookup"><span data-stu-id="2d29d-151">middle</span></span>        |<span data-ttu-id="2d29d-152">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-152">String</span></span>                                           | <span data-ttu-id="2d29d-153">Отчество пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-153">User's middle name.</span></span>                                                                     |
|<span data-ttu-id="2d29d-154">прозвищ</span><span class="sxs-lookup"><span data-stu-id="2d29d-154">nickname</span></span>      |<span data-ttu-id="2d29d-155">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-155">String</span></span>                                           | <span data-ttu-id="2d29d-156">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-156">User's nickname.</span></span>                                                                        |
|<span data-ttu-id="2d29d-157">произношение</span><span class="sxs-lookup"><span data-stu-id="2d29d-157">pronunciation</span></span> |[<span data-ttu-id="2d29d-158">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="2d29d-158">yomiPersonName</span></span>](../resources/yomipersonname.md) | <span data-ttu-id="2d29d-159">Содержит сведения о произношении имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-159">Contains details about pronunciation of the users name.</span></span>                                 |
|<span data-ttu-id="2d29d-160">суффикс</span><span class="sxs-lookup"><span data-stu-id="2d29d-160">suffix</span></span>        |<span data-ttu-id="2d29d-161">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-161">String</span></span>                                           | <span data-ttu-id="2d29d-162">Обозначения, используемые после имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-162">Designators used after the users name.</span></span> <span data-ttu-id="2d29d-163">(например, "доктор".)</span><span class="sxs-lookup"><span data-stu-id="2d29d-163">(eg: PhD.)</span></span>                                       |
|<span data-ttu-id="2d29d-164">title</span><span class="sxs-lookup"><span data-stu-id="2d29d-164">title</span></span>         |<span data-ttu-id="2d29d-165">String</span><span class="sxs-lookup"><span data-stu-id="2d29d-165">String</span></span>                                           | <span data-ttu-id="2d29d-166">Хонорификс используется для префикса имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d29d-166">Honorifics used to prefix a users name.</span></span> <span data-ttu-id="2d29d-167">(например, "доктор", "Sir", "Мадам", Mrs.)</span><span class="sxs-lookup"><span data-stu-id="2d29d-167">(eg: Dr, Sir, Madam, Mrs.)</span></span>                      |

## <a name="response"></a><span data-ttu-id="2d29d-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d29d-168">Response</span></span>

<span data-ttu-id="2d29d-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d29d-169">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d29d-170">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d29d-170">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d29d-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d29d-171">Request</span></span>

<span data-ttu-id="2d29d-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d29d-172">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2d29d-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d29d-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personname"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/names/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d29d-174">C#</span><span class="sxs-lookup"><span data-stu-id="2d29d-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d29d-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d29d-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d29d-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d29d-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2d29d-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d29d-177">Response</span></span>

<span data-ttu-id="2d29d-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d29d-178">The following is an example of the response.</span></span>

> <span data-ttu-id="2d29d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d29d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personname",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
