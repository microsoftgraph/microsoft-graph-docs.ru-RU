---
title: Обновление свойств educationclass
description: Обновление свойств курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7932dc3072689468ceff813a99466d287ce77a1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950566"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="acca3-103">Обновление свойств educationclass</span><span class="sxs-lookup"><span data-stu-id="acca3-103">Update educationclass properties</span></span>

> <span data-ttu-id="acca3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="acca3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acca3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acca3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="acca3-106">Обновление свойств курса.</span><span class="sxs-lookup"><span data-stu-id="acca3-106">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="acca3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="acca3-107">Permissions</span></span>
<span data-ttu-id="acca3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acca3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acca3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acca3-110">Permission type</span></span>      | <span data-ttu-id="acca3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="acca3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acca3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acca3-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="acca3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acca3-113">Not supported.</span></span>  |
|<span data-ttu-id="acca3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acca3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acca3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acca3-115">Not supported.</span></span>   |
|<span data-ttu-id="acca3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acca3-116">Application</span></span> | <span data-ttu-id="acca3-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acca3-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="acca3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acca3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="acca3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acca3-119">Request headers</span></span>
| <span data-ttu-id="acca3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="acca3-120">Header</span></span>       | <span data-ttu-id="acca3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="acca3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="acca3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="acca3-122">Authorization</span></span>  | <span data-ttu-id="acca3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acca3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="acca3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="acca3-125">Content-Type</span></span>  | <span data-ttu-id="acca3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acca3-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="acca3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acca3-127">Request body</span></span>
<span data-ttu-id="acca3-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="acca3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="acca3-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="acca3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="acca3-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="acca3-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="acca3-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="acca3-131">Property</span></span>     | <span data-ttu-id="acca3-132">Тип</span><span class="sxs-lookup"><span data-stu-id="acca3-132">Type</span></span>   |<span data-ttu-id="acca3-133">Описание</span><span class="sxs-lookup"><span data-stu-id="acca3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acca3-134">описание</span><span class="sxs-lookup"><span data-stu-id="acca3-134">description</span></span>|<span data-ttu-id="acca3-135">String</span><span class="sxs-lookup"><span data-stu-id="acca3-135">String</span></span>| <span data-ttu-id="acca3-136">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="acca3-136">Description of the class.</span></span>|
|<span data-ttu-id="acca3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="acca3-137">displayName</span></span>|<span data-ttu-id="acca3-138">String</span><span class="sxs-lookup"><span data-stu-id="acca3-138">String</span></span>| <span data-ttu-id="acca3-139">Название курса.</span><span class="sxs-lookup"><span data-stu-id="acca3-139">Name of the class.</span></span>|
|<span data-ttu-id="acca3-140">mailNickname</span><span class="sxs-lookup"><span data-stu-id="acca3-140">mailNickname</span></span>|<span data-ttu-id="acca3-141">String</span><span class="sxs-lookup"><span data-stu-id="acca3-141">String</span></span>| <span data-ttu-id="acca3-142">Почтовый псевдоним для отправки электронных сообщений всем пользователям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="acca3-142">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="acca3-143"><!-- Please verify the revised description here. -->| classCode | Строка | Класс код, используемый в школе. | | externalId | Строка | Идентификатор класса в системе выполняется синхронизация.</span><span class="sxs-lookup"><span data-stu-id="acca3-143"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="acca3-144">Свойство externalName типа String представляет собой название курса в системе синхронизации. Свойство externalSource типа String представляет собой способ создания курса.</span><span class="sxs-lookup"><span data-stu-id="acca3-144">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="acca3-145">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="acca3-145">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="acca3-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="acca3-146">Response</span></span>
<span data-ttu-id="acca3-147">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="acca3-147">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="acca3-148">Пример</span><span class="sxs-lookup"><span data-stu-id="acca3-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acca3-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="acca3-149">Request</span></span>
<span data-ttu-id="acca3-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acca3-150">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="acca3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="acca3-151">Response</span></span>
<span data-ttu-id="acca3-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="acca3-152">The following is an example of the response.</span></span> 

><span data-ttu-id="acca3-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="acca3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
