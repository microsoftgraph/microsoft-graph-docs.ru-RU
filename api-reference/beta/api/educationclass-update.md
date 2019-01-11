---
title: Обновление свойств educationclass
description: Обновление свойств курса.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 1c011a19371490bb8d00a7048a9809cc8a58beee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813995"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="0335c-103">Обновление свойств educationclass</span><span class="sxs-lookup"><span data-stu-id="0335c-103">Update educationclass properties</span></span>

> <span data-ttu-id="0335c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0335c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0335c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0335c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0335c-106">Обновление свойств курса.</span><span class="sxs-lookup"><span data-stu-id="0335c-106">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="0335c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0335c-107">Permissions</span></span>
<span data-ttu-id="0335c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0335c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0335c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0335c-110">Permission type</span></span>      | <span data-ttu-id="0335c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0335c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0335c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0335c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0335c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0335c-113">Not supported.</span></span>  |
|<span data-ttu-id="0335c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0335c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0335c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0335c-115">Not supported.</span></span>   |
|<span data-ttu-id="0335c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0335c-116">Application</span></span> | <span data-ttu-id="0335c-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0335c-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0335c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0335c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0335c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0335c-119">Request headers</span></span>
| <span data-ttu-id="0335c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0335c-120">Header</span></span>       | <span data-ttu-id="0335c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0335c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0335c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0335c-122">Authorization</span></span>  | <span data-ttu-id="0335c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0335c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0335c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0335c-125">Content-Type</span></span>  | <span data-ttu-id="0335c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0335c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0335c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0335c-127">Request body</span></span>
<span data-ttu-id="0335c-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0335c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0335c-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0335c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0335c-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0335c-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0335c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0335c-131">Property</span></span>     | <span data-ttu-id="0335c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0335c-132">Type</span></span>   |<span data-ttu-id="0335c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0335c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0335c-134">описание</span><span class="sxs-lookup"><span data-stu-id="0335c-134">description</span></span>|<span data-ttu-id="0335c-135">String</span><span class="sxs-lookup"><span data-stu-id="0335c-135">String</span></span>| <span data-ttu-id="0335c-136">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="0335c-136">Description of the class.</span></span>|
|<span data-ttu-id="0335c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0335c-137">displayName</span></span>|<span data-ttu-id="0335c-138">String</span><span class="sxs-lookup"><span data-stu-id="0335c-138">String</span></span>| <span data-ttu-id="0335c-139">Название курса.</span><span class="sxs-lookup"><span data-stu-id="0335c-139">Name of the class.</span></span>|
|<span data-ttu-id="0335c-140">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0335c-140">mailNickname</span></span>|<span data-ttu-id="0335c-141">String</span><span class="sxs-lookup"><span data-stu-id="0335c-141">String</span></span>| <span data-ttu-id="0335c-142">Почтовый псевдоним для отправки электронных сообщений всем пользователям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="0335c-142">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="0335c-143"><!-- Please verify the revised description here. -->| classCode | Строка | Класс код, используемый в школе. | | externalId | Строка | Идентификатор класса в системе выполняется синхронизация.</span><span class="sxs-lookup"><span data-stu-id="0335c-143"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="0335c-144">Свойство externalName типа String представляет собой название курса в системе синхронизации. Свойство externalSource типа String представляет собой способ создания курса.</span><span class="sxs-lookup"><span data-stu-id="0335c-144">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="0335c-145">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="0335c-145">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="0335c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0335c-146">Response</span></span>
<span data-ttu-id="0335c-147">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0335c-147">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0335c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="0335c-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0335c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="0335c-149">Request</span></span>
<span data-ttu-id="0335c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0335c-150">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0335c-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="0335c-151">Response</span></span>
<span data-ttu-id="0335c-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0335c-152">The following is an example of the response.</span></span> 

><span data-ttu-id="0335c-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0335c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
