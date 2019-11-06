---
title: Обновление ЛангуажепрофиЦиенци
description: Обновление свойств объекта ЛангуажепрофиЦиенци в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6d85263db9d54565613678d4941594e5df312d57
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998258"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="8c576-103">Обновление ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="8c576-103">Update languageProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c576-104">Обновление свойств объекта [лангуажепрофиЦиенци](../resources/languageproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c576-104">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c576-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c576-105">Permissions</span></span>

<span data-ttu-id="8c576-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c576-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c576-108">Permission type</span></span>                        | <span data-ttu-id="8c576-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c576-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c576-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c576-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c576-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8c576-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8c576-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c576-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c576-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8c576-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8c576-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c576-114">Application</span></span>                            | <span data-ttu-id="8c576-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c576-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8c576-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c576-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8c576-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c576-117">Request headers</span></span>

| <span data-ttu-id="8c576-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8c576-118">Name</span></span>           |<span data-ttu-id="8c576-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8c576-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="8c576-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c576-120">Authorization</span></span>  | <span data-ttu-id="8c576-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c576-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8c576-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c576-123">Content-Type</span></span>   | <span data-ttu-id="8c576-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c576-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c576-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c576-126">Request body</span></span>

<span data-ttu-id="8c576-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8c576-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8c576-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8c576-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8c576-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8c576-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8c576-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c576-130">Property</span></span>     | <span data-ttu-id="8c576-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c576-131">Type</span></span>        | <span data-ttu-id="8c576-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c576-132">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="8c576-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8c576-133">displayName</span></span>   |<span data-ttu-id="8c576-134">String</span><span class="sxs-lookup"><span data-stu-id="8c576-134">String</span></span>       | <span data-ttu-id="8c576-135">Содержит имя длинной формы для рассматриваемого языка.</span><span class="sxs-lookup"><span data-stu-id="8c576-135">Contains the long-form name for the language in question.</span></span>                                                                                                   |
|<span data-ttu-id="8c576-136">навыки</span><span class="sxs-lookup"><span data-stu-id="8c576-136">proficiency</span></span>   |<span data-ttu-id="8c576-137">string</span><span class="sxs-lookup"><span data-stu-id="8c576-137">string</span></span>       | <span data-ttu-id="8c576-138">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8c576-138">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8c576-139">tag</span><span class="sxs-lookup"><span data-stu-id="8c576-139">tag</span></span>           |<span data-ttu-id="8c576-140">String</span><span class="sxs-lookup"><span data-stu-id="8c576-140">String</span></span>       | <span data-ttu-id="8c576-141">Содержит 4-символьное имя BCP47 для языка (EN-US, No-NetBIOS, en-AU)</span><span class="sxs-lookup"><span data-stu-id="8c576-141">Contains the 4 character BCP47 name for the language (en-US, no-NB, en-AU)</span></span>                                                                                  |

## <a name="response"></a><span data-ttu-id="8c576-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c576-142">Response</span></span>

<span data-ttu-id="8c576-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [лангуажепрофиЦиенци](../resources/languageproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c576-143">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c576-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c576-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c576-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c576-145">Request</span></span>

<span data-ttu-id="8c576-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c576-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c576-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c576-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c576-148">C#</span><span class="sxs-lookup"><span data-stu-id="8c576-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c576-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c576-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c576-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c576-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c576-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c576-151">Response</span></span>

<span data-ttu-id="8c576-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c576-152">The following is an example of the response.</span></span>

> <span data-ttu-id="8c576-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c576-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
