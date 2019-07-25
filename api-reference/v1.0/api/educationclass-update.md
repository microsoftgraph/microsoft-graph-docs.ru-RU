---
title: Обновление свойств educationclass
description: Обновление свойств курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ac3ce20d4536a37d56988d72a0bbf69ff691930d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881504"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="fad97-103">Обновление свойств educationclass</span><span class="sxs-lookup"><span data-stu-id="fad97-103">Update educationclass properties</span></span>

<span data-ttu-id="fad97-104">Обновление свойств курса.</span><span class="sxs-lookup"><span data-stu-id="fad97-104">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="fad97-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fad97-105">Permissions</span></span>
<span data-ttu-id="fad97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fad97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fad97-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fad97-108">Permission type</span></span>      | <span data-ttu-id="fad97-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fad97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fad97-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fad97-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fad97-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fad97-111">Not supported.</span></span>  |
|<span data-ttu-id="fad97-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fad97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fad97-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fad97-113">Not supported.</span></span>   |
|<span data-ttu-id="fad97-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fad97-114">Application</span></span> | <span data-ttu-id="fad97-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad97-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fad97-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fad97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fad97-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fad97-117">Request headers</span></span>
| <span data-ttu-id="fad97-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fad97-118">Header</span></span>       | <span data-ttu-id="fad97-119">Значение</span><span class="sxs-lookup"><span data-stu-id="fad97-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fad97-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fad97-120">Authorization</span></span>  | <span data-ttu-id="fad97-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fad97-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fad97-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fad97-123">Content-Type</span></span>  | <span data-ttu-id="fad97-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fad97-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fad97-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fad97-125">Request body</span></span>
<span data-ttu-id="fad97-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="fad97-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="fad97-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="fad97-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fad97-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fad97-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fad97-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fad97-129">Property</span></span>     | <span data-ttu-id="fad97-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fad97-130">Type</span></span>   |<span data-ttu-id="fad97-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fad97-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fad97-132">description</span><span class="sxs-lookup"><span data-stu-id="fad97-132">description</span></span>|<span data-ttu-id="fad97-133">String</span><span class="sxs-lookup"><span data-stu-id="fad97-133">String</span></span>| <span data-ttu-id="fad97-134">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="fad97-134">Description of the class.</span></span>|
|<span data-ttu-id="fad97-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fad97-135">displayName</span></span>|<span data-ttu-id="fad97-136">Строка</span><span class="sxs-lookup"><span data-stu-id="fad97-136">String</span></span>| <span data-ttu-id="fad97-137">Название курса.</span><span class="sxs-lookup"><span data-stu-id="fad97-137">Name of the class.</span></span>|
|<span data-ttu-id="fad97-138">mailNickname</span><span class="sxs-lookup"><span data-stu-id="fad97-138">mailNickname</span></span>|<span data-ttu-id="fad97-139">String</span><span class="sxs-lookup"><span data-stu-id="fad97-139">String</span></span>| <span data-ttu-id="fad97-140">Почтовый псевдоним для отправки электронных сообщений всем пользователям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="fad97-140">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="fad97-141">Свойство classCode типа String представляет собой код курса, используемый учебным заведением. Свойство externalId типа String представляет собой идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fad97-141">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="fad97-142">Свойство externalName типа String представляет собой название курса в системе синхронизации. Свойство externalSource типа String представляет собой способ создания курса.</span><span class="sxs-lookup"><span data-stu-id="fad97-142">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="fad97-143">Возможные значения: `sis`, `manual`, `enum_sentinel`. |</span><span class="sxs-lookup"><span data-stu-id="fad97-143">The possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="fad97-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fad97-144">Response</span></span>
<span data-ttu-id="fad97-145">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fad97-145">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fad97-146">Пример</span><span class="sxs-lookup"><span data-stu-id="fad97-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fad97-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="fad97-147">Request</span></span>
<span data-ttu-id="fad97-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fad97-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fad97-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="fad97-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fad97-150">C#</span><span class="sxs-lookup"><span data-stu-id="fad97-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fad97-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="fad97-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fad97-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fad97-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fad97-153">Java</span><span class="sxs-lookup"><span data-stu-id="fad97-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fad97-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="fad97-154">Response</span></span>
<span data-ttu-id="fad97-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fad97-155">The following is an example of the response.</span></span> 

><span data-ttu-id="fad97-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fad97-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
