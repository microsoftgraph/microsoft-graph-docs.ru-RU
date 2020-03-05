---
title: Обновление свойств educationclass
description: Обновление свойств курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7e2ee8f1da830253f8f8d8a2ada0d8ec8b0c029f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426306"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="eef7e-103">Обновление свойств educationclass</span><span class="sxs-lookup"><span data-stu-id="eef7e-103">Update educationclass properties</span></span>

<span data-ttu-id="eef7e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eef7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eef7e-105">Обновление свойств курса.</span><span class="sxs-lookup"><span data-stu-id="eef7e-105">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="eef7e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eef7e-106">Permissions</span></span>
<span data-ttu-id="eef7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eef7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eef7e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eef7e-109">Permission type</span></span>      | <span data-ttu-id="eef7e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eef7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eef7e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eef7e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="eef7e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef7e-112">Not supported.</span></span>  |
|<span data-ttu-id="eef7e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eef7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eef7e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eef7e-114">Not supported.</span></span>   |
|<span data-ttu-id="eef7e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eef7e-115">Application</span></span> | <span data-ttu-id="eef7e-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef7e-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="eef7e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eef7e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eef7e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eef7e-118">Request headers</span></span>
| <span data-ttu-id="eef7e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eef7e-119">Header</span></span>       | <span data-ttu-id="eef7e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="eef7e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eef7e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eef7e-121">Authorization</span></span>  | <span data-ttu-id="eef7e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eef7e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eef7e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eef7e-124">Content-Type</span></span>  | <span data-ttu-id="eef7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eef7e-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eef7e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eef7e-126">Request body</span></span>
<span data-ttu-id="eef7e-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="eef7e-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="eef7e-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="eef7e-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eef7e-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="eef7e-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eef7e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eef7e-130">Property</span></span>     | <span data-ttu-id="eef7e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eef7e-131">Type</span></span>   |<span data-ttu-id="eef7e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eef7e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eef7e-133">description</span><span class="sxs-lookup"><span data-stu-id="eef7e-133">description</span></span>|<span data-ttu-id="eef7e-134">String</span><span class="sxs-lookup"><span data-stu-id="eef7e-134">String</span></span>| <span data-ttu-id="eef7e-135">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="eef7e-135">Description of the class.</span></span>|
|<span data-ttu-id="eef7e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eef7e-136">displayName</span></span>|<span data-ttu-id="eef7e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="eef7e-137">String</span></span>| <span data-ttu-id="eef7e-138">Название курса.</span><span class="sxs-lookup"><span data-stu-id="eef7e-138">Name of the class.</span></span>|
|<span data-ttu-id="eef7e-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="eef7e-139">mailNickname</span></span>|<span data-ttu-id="eef7e-140">String</span><span class="sxs-lookup"><span data-stu-id="eef7e-140">String</span></span>| <span data-ttu-id="eef7e-141">Почтовый псевдоним для отправки электронных сообщений всем пользователям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="eef7e-141">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="eef7e-142">Свойство classCode типа String представляет собой код курса, используемый учебным заведением. Свойство externalId типа String представляет собой идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="eef7e-142">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="eef7e-143">Свойство externalName типа String представляет собой название курса в системе синхронизации. Свойство externalSource типа String представляет собой способ создания курса.</span><span class="sxs-lookup"><span data-stu-id="eef7e-143">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="eef7e-144">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="eef7e-144">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="eef7e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="eef7e-145">Response</span></span>
<span data-ttu-id="eef7e-146">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eef7e-146">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eef7e-147">Пример</span><span class="sxs-lookup"><span data-stu-id="eef7e-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eef7e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="eef7e-148">Request</span></span>
<span data-ttu-id="eef7e-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eef7e-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eef7e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="eef7e-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eef7e-151">C#</span><span class="sxs-lookup"><span data-stu-id="eef7e-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eef7e-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eef7e-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eef7e-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eef7e-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eef7e-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="eef7e-154">Response</span></span>
<span data-ttu-id="eef7e-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eef7e-155">The following is an example of the response.</span></span> 

><span data-ttu-id="eef7e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eef7e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
