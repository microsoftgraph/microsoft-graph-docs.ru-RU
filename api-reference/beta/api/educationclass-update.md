---
title: Обновление свойств educationclass
description: Обновление свойств курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1ca407ab560f70ae0d65252e397705cb878e0f52
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457762"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="6b04f-103">Обновление свойств educationclass</span><span class="sxs-lookup"><span data-stu-id="6b04f-103">Update educationclass properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b04f-104">Обновление свойств курса.</span><span class="sxs-lookup"><span data-stu-id="6b04f-104">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b04f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b04f-105">Permissions</span></span>
<span data-ttu-id="6b04f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b04f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b04f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b04f-108">Permission type</span></span>      | <span data-ttu-id="6b04f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b04f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b04f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b04f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6b04f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b04f-111">Not supported.</span></span>  |
|<span data-ttu-id="6b04f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b04f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b04f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b04f-113">Not supported.</span></span>   |
|<span data-ttu-id="6b04f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b04f-114">Application</span></span> | <span data-ttu-id="6b04f-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b04f-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6b04f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b04f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6b04f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b04f-117">Request headers</span></span>
| <span data-ttu-id="6b04f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b04f-118">Header</span></span>       | <span data-ttu-id="6b04f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="6b04f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b04f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b04f-120">Authorization</span></span>  | <span data-ttu-id="6b04f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b04f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6b04f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b04f-123">Content-Type</span></span>  | <span data-ttu-id="6b04f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6b04f-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b04f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b04f-125">Request body</span></span>
<span data-ttu-id="6b04f-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6b04f-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6b04f-127">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="6b04f-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6b04f-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6b04f-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6b04f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b04f-129">Property</span></span>     | <span data-ttu-id="6b04f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6b04f-130">Type</span></span>   |<span data-ttu-id="6b04f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6b04f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b04f-132">description</span><span class="sxs-lookup"><span data-stu-id="6b04f-132">description</span></span>|<span data-ttu-id="6b04f-133">String</span><span class="sxs-lookup"><span data-stu-id="6b04f-133">String</span></span>| <span data-ttu-id="6b04f-134">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="6b04f-134">Description of the class.</span></span>|
|<span data-ttu-id="6b04f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6b04f-135">displayName</span></span>|<span data-ttu-id="6b04f-136">Строка</span><span class="sxs-lookup"><span data-stu-id="6b04f-136">String</span></span>| <span data-ttu-id="6b04f-137">Название курса.</span><span class="sxs-lookup"><span data-stu-id="6b04f-137">Name of the class.</span></span>|
|<span data-ttu-id="6b04f-138">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6b04f-138">mailNickname</span></span>|<span data-ttu-id="6b04f-139">String</span><span class="sxs-lookup"><span data-stu-id="6b04f-139">String</span></span>| <span data-ttu-id="6b04f-140">Почтовый псевдоним для отправки электронных сообщений всем пользователям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="6b04f-140">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="6b04f-141">Свойство classCode типа String представляет собой код курса, используемый учебным заведением. Свойство externalId типа String представляет собой идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="6b04f-141">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="6b04f-142">Свойство externalName типа String представляет собой название курса в системе синхронизации. Свойство externalSource типа String представляет собой способ создания курса.</span><span class="sxs-lookup"><span data-stu-id="6b04f-142">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="6b04f-143">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="6b04f-143">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="6b04f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b04f-144">Response</span></span>
<span data-ttu-id="6b04f-145">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6b04f-145">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b04f-146">Пример</span><span class="sxs-lookup"><span data-stu-id="6b04f-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b04f-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b04f-147">Request</span></span>
<span data-ttu-id="6b04f-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b04f-148">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6b04f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b04f-149">Response</span></span>
<span data-ttu-id="6b04f-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b04f-150">The following is an example of the response.</span></span> 

><span data-ttu-id="6b04f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b04f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/educationclass-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
