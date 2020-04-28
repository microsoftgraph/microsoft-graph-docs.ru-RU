---
title: Обновление ЛангуажепрофиЦиенци
description: Обновление свойств объекта ЛангуажепрофиЦиенци в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5f9dcea968f3dde36de2ba46dc8c29c5c584a198
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228925"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="1cc07-103">Обновление ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="1cc07-103">Update languageProficiency</span></span>

<span data-ttu-id="1cc07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cc07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc07-105">Обновление свойств объекта [лангуажепрофиЦиенци](../resources/languageproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cc07-105">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc07-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cc07-106">Permissions</span></span>

<span data-ttu-id="1cc07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cc07-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cc07-109">Permission type</span></span>                        | <span data-ttu-id="1cc07-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cc07-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1cc07-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cc07-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cc07-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1cc07-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1cc07-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cc07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc07-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1cc07-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1cc07-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cc07-115">Application</span></span>                            | <span data-ttu-id="1cc07-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cc07-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1cc07-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cc07-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1cc07-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cc07-118">Request headers</span></span>

| <span data-ttu-id="1cc07-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1cc07-119">Name</span></span>           |<span data-ttu-id="1cc07-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1cc07-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1cc07-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cc07-121">Authorization</span></span>  | <span data-ttu-id="1cc07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cc07-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1cc07-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1cc07-124">Content-Type</span></span>   | <span data-ttu-id="1cc07-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cc07-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cc07-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cc07-127">Request body</span></span>

<span data-ttu-id="1cc07-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1cc07-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1cc07-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1cc07-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1cc07-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1cc07-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1cc07-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cc07-131">Property</span></span>     | <span data-ttu-id="1cc07-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1cc07-132">Type</span></span>        | <span data-ttu-id="1cc07-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1cc07-133">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="1cc07-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1cc07-134">displayName</span></span>   |<span data-ttu-id="1cc07-135">String</span><span class="sxs-lookup"><span data-stu-id="1cc07-135">String</span></span>       | <span data-ttu-id="1cc07-136">Содержит имя длинной формы для рассматриваемого языка.</span><span class="sxs-lookup"><span data-stu-id="1cc07-136">Contains the long-form name for the language in question.</span></span>                                                                                                   |
|<span data-ttu-id="1cc07-137">навыки</span><span class="sxs-lookup"><span data-stu-id="1cc07-137">proficiency</span></span>   |<span data-ttu-id="1cc07-138">string</span><span class="sxs-lookup"><span data-stu-id="1cc07-138">string</span></span>       | <span data-ttu-id="1cc07-139">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1cc07-139">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1cc07-140">tag</span><span class="sxs-lookup"><span data-stu-id="1cc07-140">tag</span></span>           |<span data-ttu-id="1cc07-141">String</span><span class="sxs-lookup"><span data-stu-id="1cc07-141">String</span></span>       | <span data-ttu-id="1cc07-142">Содержит 4-символьное имя BCP47 для языка (EN-US, No-NetBIOS, en-AU)</span><span class="sxs-lookup"><span data-stu-id="1cc07-142">Contains the 4 character BCP47 name for the language (en-US, no-NB, en-AU)</span></span>                                                                                  |

## <a name="response"></a><span data-ttu-id="1cc07-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cc07-143">Response</span></span>

<span data-ttu-id="1cc07-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [лангуажепрофиЦиенци](../resources/languageproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1cc07-144">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1cc07-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="1cc07-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1cc07-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cc07-146">Request</span></span>

<span data-ttu-id="1cc07-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cc07-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1cc07-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc07-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_languageproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/languages/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1cc07-149">C#</span><span class="sxs-lookup"><span data-stu-id="1cc07-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cc07-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cc07-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cc07-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cc07-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1cc07-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cc07-152">Response</span></span>

<span data-ttu-id="1cc07-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1cc07-153">The following is an example of the response.</span></span>

> <span data-ttu-id="1cc07-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cc07-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update languageproficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
