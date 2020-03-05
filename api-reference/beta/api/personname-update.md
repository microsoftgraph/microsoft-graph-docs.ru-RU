---
title: Обновление personName
description: Обновление свойств объекта PersonName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ef65c81830c219d988159753be3528d37609c531
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455892"
---
# <a name="update-personname"></a><span data-ttu-id="4571f-103">Обновление PersonName</span><span class="sxs-lookup"><span data-stu-id="4571f-103">Update personname</span></span>

<span data-ttu-id="4571f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4571f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4571f-105">Обновление свойств объекта [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-105">Update the properties of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4571f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4571f-106">Permissions</span></span>

<span data-ttu-id="4571f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4571f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4571f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4571f-109">Permission type</span></span>                        | <span data-ttu-id="4571f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4571f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4571f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4571f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4571f-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4571f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4571f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4571f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4571f-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4571f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4571f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4571f-115">Application</span></span>                            | <span data-ttu-id="4571f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4571f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4571f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4571f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4571f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4571f-118">Request headers</span></span>

| <span data-ttu-id="4571f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4571f-119">Name</span></span>           |<span data-ttu-id="4571f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4571f-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4571f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4571f-121">Authorization</span></span>  | <span data-ttu-id="4571f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4571f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4571f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4571f-124">Content-Type</span></span>   | <span data-ttu-id="4571f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4571f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4571f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4571f-127">Request body</span></span>

<span data-ttu-id="4571f-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4571f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4571f-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4571f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4571f-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4571f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4571f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4571f-131">Property</span></span>     | <span data-ttu-id="4571f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4571f-132">Type</span></span>                                            | <span data-ttu-id="4571f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4571f-133">Description</span></span>                                                                             | 
|:-------------|:------------------------------------------------|:----------------------------------------------------------------------------------------|
|<span data-ttu-id="4571f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4571f-134">displayName</span></span>   |<span data-ttu-id="4571f-135">Строка</span><span class="sxs-lookup"><span data-stu-id="4571f-135">String</span></span>                                           | <span data-ttu-id="4571f-136">Предоставляет упорядоченную визуализацию имени и фамилии.</span><span class="sxs-lookup"><span data-stu-id="4571f-136">Provides an ordered rendering of first name and last name.</span></span>                              |
|<span data-ttu-id="4571f-137">первыми</span><span class="sxs-lookup"><span data-stu-id="4571f-137">first</span></span>         |<span data-ttu-id="4571f-138">String</span><span class="sxs-lookup"><span data-stu-id="4571f-138">String</span></span>                                           | <span data-ttu-id="4571f-139">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-139">First Name of the user.</span></span>                                                                 |
|<span data-ttu-id="4571f-140">initials</span><span class="sxs-lookup"><span data-stu-id="4571f-140">initials</span></span>      |<span data-ttu-id="4571f-141">String</span><span class="sxs-lookup"><span data-stu-id="4571f-141">String</span></span>                                           | <span data-ttu-id="4571f-142">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-142">Initials of the user.</span></span>                                                                   |
|<span data-ttu-id="4571f-143">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="4571f-143">languageTag</span></span>   |<span data-ttu-id="4571f-144">String</span><span class="sxs-lookup"><span data-stu-id="4571f-144">String</span></span>                                           | <span data-ttu-id="4571f-145">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="4571f-145">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>   |
|<span data-ttu-id="4571f-146">Фамили</span><span class="sxs-lookup"><span data-stu-id="4571f-146">last</span></span>          |<span data-ttu-id="4571f-147">String</span><span class="sxs-lookup"><span data-stu-id="4571f-147">String</span></span>                                           | <span data-ttu-id="4571f-148">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-148">Last name of the user.</span></span>                                                                  |
|<span data-ttu-id="4571f-149">маиден</span><span class="sxs-lookup"><span data-stu-id="4571f-149">maiden</span></span>        |<span data-ttu-id="4571f-150">String</span><span class="sxs-lookup"><span data-stu-id="4571f-150">String</span></span>                                           | <span data-ttu-id="4571f-151">Имя пользователя, марриаже фамилию.</span><span class="sxs-lookup"><span data-stu-id="4571f-151">User's pre-marriage last name.</span></span>                                                          |
|<span data-ttu-id="4571f-152">назван</span><span class="sxs-lookup"><span data-stu-id="4571f-152">middle</span></span>        |<span data-ttu-id="4571f-153">String</span><span class="sxs-lookup"><span data-stu-id="4571f-153">String</span></span>                                           | <span data-ttu-id="4571f-154">Отчество пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-154">User's middle name.</span></span>                                                                     |
|<span data-ttu-id="4571f-155">прозвищ</span><span class="sxs-lookup"><span data-stu-id="4571f-155">nickname</span></span>      |<span data-ttu-id="4571f-156">String</span><span class="sxs-lookup"><span data-stu-id="4571f-156">String</span></span>                                           | <span data-ttu-id="4571f-157">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-157">User's nickname.</span></span>                                                                        |
|<span data-ttu-id="4571f-158">произношение</span><span class="sxs-lookup"><span data-stu-id="4571f-158">pronunciation</span></span> |[<span data-ttu-id="4571f-159">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="4571f-159">yomiPersonName</span></span>](../resources/yomipersonname.md) | <span data-ttu-id="4571f-160">Содержит сведения о произношении имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-160">Contains details about pronunciation of the users name.</span></span>                                 |
|<span data-ttu-id="4571f-161">суффикс</span><span class="sxs-lookup"><span data-stu-id="4571f-161">suffix</span></span>        |<span data-ttu-id="4571f-162">String</span><span class="sxs-lookup"><span data-stu-id="4571f-162">String</span></span>                                           | <span data-ttu-id="4571f-163">Обозначения, используемые после имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-163">Designators used after the users name.</span></span> <span data-ttu-id="4571f-164">(например, "доктор".)</span><span class="sxs-lookup"><span data-stu-id="4571f-164">(eg: PhD.)</span></span>                                       |
|<span data-ttu-id="4571f-165">title</span><span class="sxs-lookup"><span data-stu-id="4571f-165">title</span></span>         |<span data-ttu-id="4571f-166">String</span><span class="sxs-lookup"><span data-stu-id="4571f-166">String</span></span>                                           | <span data-ttu-id="4571f-167">Хонорификс используется для префикса имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4571f-167">Honorifics used to prefix a users name.</span></span> <span data-ttu-id="4571f-168">(например, "доктор", "Sir", "Мадам", Mrs.)</span><span class="sxs-lookup"><span data-stu-id="4571f-168">(eg: Dr, Sir, Madam, Mrs.)</span></span>                      |

## <a name="response"></a><span data-ttu-id="4571f-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="4571f-169">Response</span></span>

<span data-ttu-id="4571f-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4571f-170">If successful, this method returns a `200 OK` response code and an updated [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4571f-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="4571f-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4571f-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="4571f-172">Request</span></span>

<span data-ttu-id="4571f-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4571f-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4571f-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="4571f-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4571f-175">C#</span><span class="sxs-lookup"><span data-stu-id="4571f-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4571f-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4571f-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4571f-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4571f-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4571f-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="4571f-178">Response</span></span>

<span data-ttu-id="4571f-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4571f-179">The following is an example of the response.</span></span>

> <span data-ttu-id="4571f-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4571f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
