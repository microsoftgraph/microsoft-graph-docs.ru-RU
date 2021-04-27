---
title: Обновление свойств educationclass
description: Обновление свойств курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 425d2072e13dbf00d8fc2e81b94cf7da58df8c57
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043733"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="1b8eb-103">Обновление свойств educationclass</span><span class="sxs-lookup"><span data-stu-id="1b8eb-103">Update educationclass properties</span></span>

<span data-ttu-id="1b8eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b8eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b8eb-105">Обновление свойств курса.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-105">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b8eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b8eb-106">Permissions</span></span>
<span data-ttu-id="1b8eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b8eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b8eb-109">Permission type</span></span>      | <span data-ttu-id="1b8eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b8eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b8eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b8eb-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1b8eb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-112">Not supported.</span></span>  |
|<span data-ttu-id="1b8eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b8eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b8eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-114">Not supported.</span></span>   |
|<span data-ttu-id="1b8eb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b8eb-115">Application</span></span> | <span data-ttu-id="1b8eb-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b8eb-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b8eb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b8eb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1b8eb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b8eb-118">Request headers</span></span>
| <span data-ttu-id="1b8eb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b8eb-119">Header</span></span>       | <span data-ttu-id="1b8eb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1b8eb-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b8eb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b8eb-121">Authorization</span></span>  | <span data-ttu-id="1b8eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b8eb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b8eb-124">Content-Type</span></span>  | <span data-ttu-id="1b8eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b8eb-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b8eb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b8eb-126">Request body</span></span>
<span data-ttu-id="1b8eb-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1b8eb-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1b8eb-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1b8eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b8eb-130">Property</span></span>     | <span data-ttu-id="1b8eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1b8eb-131">Type</span></span>   |<span data-ttu-id="1b8eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1b8eb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b8eb-133">description</span><span class="sxs-lookup"><span data-stu-id="1b8eb-133">description</span></span>|<span data-ttu-id="1b8eb-134">String</span><span class="sxs-lookup"><span data-stu-id="1b8eb-134">String</span></span>| <span data-ttu-id="1b8eb-135">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-135">Description of the class.</span></span>|
|<span data-ttu-id="1b8eb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1b8eb-136">displayName</span></span>|<span data-ttu-id="1b8eb-137">String</span><span class="sxs-lookup"><span data-stu-id="1b8eb-137">String</span></span>| <span data-ttu-id="1b8eb-138">Название курса.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-138">Name of the class.</span></span>|
|<span data-ttu-id="1b8eb-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1b8eb-139">mailNickname</span></span>|<span data-ttu-id="1b8eb-140">String</span><span class="sxs-lookup"><span data-stu-id="1b8eb-140">String</span></span>| <span data-ttu-id="1b8eb-141">Почтовый псевдоним для отправки электронных сообщений всем пользователям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-141">Email alias for sending email to all users if that feature is enabled.</span></span> |
|<span data-ttu-id="1b8eb-142">classCode</span><span class="sxs-lookup"><span data-stu-id="1b8eb-142">classCode</span></span>|<span data-ttu-id="1b8eb-143">String</span><span class="sxs-lookup"><span data-stu-id="1b8eb-143">String</span></span>| <span data-ttu-id="1b8eb-144">Код класса, используемый школой.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-144">Class code used by the school.</span></span>|
|<span data-ttu-id="1b8eb-145">externalId</span><span class="sxs-lookup"><span data-stu-id="1b8eb-145">externalId</span></span>|<span data-ttu-id="1b8eb-146">String</span><span class="sxs-lookup"><span data-stu-id="1b8eb-146">String</span></span>| <span data-ttu-id="1b8eb-147">Идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-147">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="1b8eb-148">externalName</span><span class="sxs-lookup"><span data-stu-id="1b8eb-148">externalName</span></span>|<span data-ttu-id="1b8eb-149">String</span><span class="sxs-lookup"><span data-stu-id="1b8eb-149">String</span></span>|<span data-ttu-id="1b8eb-150">Название курса в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-150">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="1b8eb-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="1b8eb-151">externalSource</span></span>|<span data-ttu-id="1b8eb-152">string</span><span class="sxs-lookup"><span data-stu-id="1b8eb-152">string</span></span>| <span data-ttu-id="1b8eb-153">Способ создания этого курса.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-153">How this class was created.</span></span> <span data-ttu-id="1b8eb-154">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|

## <a name="response"></a><span data-ttu-id="1b8eb-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b8eb-155">Response</span></span>
<span data-ttu-id="1b8eb-156">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-156">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b8eb-157">Пример</span><span class="sxs-lookup"><span data-stu-id="1b8eb-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b8eb-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b8eb-158">Request</span></span>
<span data-ttu-id="1b8eb-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b8eb-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b8eb-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
# <a name="c"></a>[<span data-ttu-id="1b8eb-161">C#</span><span class="sxs-lookup"><span data-stu-id="1b8eb-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b8eb-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b8eb-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b8eb-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b8eb-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b8eb-164">Java</span><span class="sxs-lookup"><span data-stu-id="1b8eb-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1b8eb-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b8eb-165">Response</span></span>
<span data-ttu-id="1b8eb-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-166">The following is an example of the response.</span></span>

><span data-ttu-id="1b8eb-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1b8eb-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


