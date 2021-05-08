---
title: Update educationClass
description: Обновление свойств курса.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5340a05df5068942c2f895c9858e2f5cd280e24a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231964"
---
# <a name="update-educationclass"></a><span data-ttu-id="cf9e1-103">Update educationClass</span><span class="sxs-lookup"><span data-stu-id="cf9e1-103">Update educationClass</span></span>

<span data-ttu-id="cf9e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf9e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf9e1-105">Обновление свойств объекта [educationClass.](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="cf9e1-105">Update the properties of an [educationClass](../resources/educationclass.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf9e1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf9e1-106">Permissions</span></span>
<span data-ttu-id="cf9e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf9e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf9e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf9e1-109">Permission type</span></span>      | <span data-ttu-id="cf9e1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf9e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf9e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf9e1-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="cf9e1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-112">Not supported.</span></span>  |
|<span data-ttu-id="cf9e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf9e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf9e1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-114">Not supported.</span></span>   |
|<span data-ttu-id="cf9e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf9e1-115">Application</span></span> | <span data-ttu-id="cf9e1-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf9e1-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cf9e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf9e1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cf9e1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf9e1-118">Request headers</span></span>
| <span data-ttu-id="cf9e1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf9e1-119">Header</span></span>       | <span data-ttu-id="cf9e1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cf9e1-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf9e1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf9e1-121">Authorization</span></span>  | <span data-ttu-id="cf9e1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cf9e1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf9e1-124">Content-Type</span></span>  | <span data-ttu-id="cf9e1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf9e1-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf9e1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf9e1-126">Request body</span></span>
<span data-ttu-id="cf9e1-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cf9e1-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cf9e1-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cf9e1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf9e1-130">Property</span></span>             | <span data-ttu-id="cf9e1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf9e1-131">Type</span></span>                                               | <span data-ttu-id="cf9e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf9e1-132">Description</span></span>                                                        |
| :------------------- | :------------------------------------------------- | :----------------------------------------------------------------- |
| <span data-ttu-id="cf9e1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cf9e1-133">displayName</span></span>          | <span data-ttu-id="cf9e1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cf9e1-134">String</span></span>                                             | <span data-ttu-id="cf9e1-135">Название курса.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-135">Name of the class.</span></span>                                                 |
| <span data-ttu-id="cf9e1-136">mailNickname</span><span class="sxs-lookup"><span data-stu-id="cf9e1-136">mailNickname</span></span>         | <span data-ttu-id="cf9e1-137">String</span><span class="sxs-lookup"><span data-stu-id="cf9e1-137">String</span></span>                                             | <span data-ttu-id="cf9e1-138">Почтовое имя для отправки почты всем участникам, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-138">Mail name for sending email to all members, if this is enabled.</span></span>    |
| <span data-ttu-id="cf9e1-139">description</span><span class="sxs-lookup"><span data-stu-id="cf9e1-139">description</span></span>          | <span data-ttu-id="cf9e1-140">Строка</span><span class="sxs-lookup"><span data-stu-id="cf9e1-140">String</span></span>                                             | <span data-ttu-id="cf9e1-141">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-141">Description of the class.</span></span>                                          |
| <span data-ttu-id="cf9e1-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="cf9e1-142">createdBy</span></span>            | [<span data-ttu-id="cf9e1-143">identitySet</span><span class="sxs-lookup"><span data-stu-id="cf9e1-143">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="cf9e1-144">Объект, который создал курс.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-144">Entity who created the class</span></span>                                       |
| <span data-ttu-id="cf9e1-145">classCode</span><span class="sxs-lookup"><span data-stu-id="cf9e1-145">classCode</span></span>            | <span data-ttu-id="cf9e1-146">String</span><span class="sxs-lookup"><span data-stu-id="cf9e1-146">String</span></span>                                             | <span data-ttu-id="cf9e1-147">Код курса, используемый учебным заведением для идентификации курса.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-147">Class code used by the school to identify the class.</span></span>               |
| <span data-ttu-id="cf9e1-148">externalId</span><span class="sxs-lookup"><span data-stu-id="cf9e1-148">externalId</span></span>           | <span data-ttu-id="cf9e1-149">String</span><span class="sxs-lookup"><span data-stu-id="cf9e1-149">String</span></span>                                             | <span data-ttu-id="cf9e1-150">Идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-150">ID of the class from the syncing system.</span></span>                           |
| <span data-ttu-id="cf9e1-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="cf9e1-151">externalSource</span></span>       | <span data-ttu-id="cf9e1-152">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="cf9e1-152">educationExternalSource</span></span>                            | <span data-ttu-id="cf9e1-153">Способ создания этого курса.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-153">How this class was created.</span></span> <span data-ttu-id="cf9e1-154">Возможные значения: `sis` , `manual`</span><span class="sxs-lookup"><span data-stu-id="cf9e1-154">Possible values are: `sis`, `manual`</span></span>   |
| <span data-ttu-id="cf9e1-155">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="cf9e1-155">externalSourceDetail</span></span> | <span data-ttu-id="cf9e1-156">Строка</span><span class="sxs-lookup"><span data-stu-id="cf9e1-156">String</span></span>                                             | <span data-ttu-id="cf9e1-157">Имя внешнего источника, из которого были созданы эти ресурсы.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-157">The name of the external source this resources was generated from.</span></span> |
| <span data-ttu-id="cf9e1-158">оценка</span><span class="sxs-lookup"><span data-stu-id="cf9e1-158">grade</span></span>                | <span data-ttu-id="cf9e1-159">String</span><span class="sxs-lookup"><span data-stu-id="cf9e1-159">String</span></span>                                             | <span data-ttu-id="cf9e1-160">Уровень класса.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-160">Grade level of the class.</span></span>                                          |
| <span data-ttu-id="cf9e1-161">term</span><span class="sxs-lookup"><span data-stu-id="cf9e1-161">term</span></span>                 | [<span data-ttu-id="cf9e1-162">educationTerm</span><span class="sxs-lookup"><span data-stu-id="cf9e1-162">educationTerm</span></span>](../resources/educationterm.md)     | <span data-ttu-id="cf9e1-163">Срок для этого курса.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-163">Term for this class.</span></span>                                               |

## <a name="response"></a><span data-ttu-id="cf9e1-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf9e1-164">Response</span></span>
<span data-ttu-id="cf9e1-165">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-165">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf9e1-166">Пример</span><span class="sxs-lookup"><span data-stu-id="cf9e1-166">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf9e1-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf9e1-167">Request</span></span>
<span data-ttu-id="cf9e1-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf9e1-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf9e1-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/{class-id}
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
# <a name="c"></a>[<span data-ttu-id="cf9e1-170">C#</span><span class="sxs-lookup"><span data-stu-id="cf9e1-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf9e1-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf9e1-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf9e1-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf9e1-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf9e1-173">Java</span><span class="sxs-lookup"><span data-stu-id="cf9e1-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cf9e1-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf9e1-174">Response</span></span>
<span data-ttu-id="cf9e1-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-175">The following is an example of the response.</span></span> 

><span data-ttu-id="cf9e1-176">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cf9e1-176">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
