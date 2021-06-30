---
title: Обновление командной работы
description: Обновление свойств объекта teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 93e78b863c0b03f475c0d6e52a12316d4eee580d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210121"
---
# <a name="update-teamworktag"></a><span data-ttu-id="8cc6b-103">Обновление командной работы</span><span class="sxs-lookup"><span data-stu-id="8cc6b-103">Update teamworkTag</span></span>
<span data-ttu-id="8cc6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc6b-105">Обновление свойств объекта [teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="8cc6b-105">Update the properties of a [teamworkTag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc6b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cc6b-106">Permissions</span></span>
<span data-ttu-id="8cc6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc6b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cc6b-109">Permission type</span></span>|<span data-ttu-id="8cc6b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cc6b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc6b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cc6b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc6b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc6b-112">Not supported.</span></span>|
|<span data-ttu-id="8cc6b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cc6b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc6b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc6b-114">Not supported.</span></span>|
|<span data-ttu-id="8cc6b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8cc6b-115">Application</span></span>|<span data-ttu-id="8cc6b-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc6b-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc6b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cc6b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="8cc6b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cc6b-118">Request headers</span></span>
|<span data-ttu-id="8cc6b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8cc6b-119">Name</span></span>|<span data-ttu-id="8cc6b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc6b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8cc6b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cc6b-121">Authorization</span></span>|<span data-ttu-id="8cc6b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cc6b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8cc6b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cc6b-124">Content-Type</span></span>|<span data-ttu-id="8cc6b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cc6b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc6b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cc6b-127">Request body</span></span>
<span data-ttu-id="8cc6b-128">В теле запроса поставляем представление JSON объекта [teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="8cc6b-128">In the request body, supply a JSON representation of the [teamworkTag](../resources/teamworktag.md) object.</span></span>

<span data-ttu-id="8cc6b-129">В следующей таблице показаны свойства, необходимые при обновлении [teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="8cc6b-129">The following table shows the properties that are required when you update the [teamworkTag](../resources/teamworktag.md).</span></span>

|<span data-ttu-id="8cc6b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cc6b-130">Property</span></span>|<span data-ttu-id="8cc6b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8cc6b-131">Type</span></span>|<span data-ttu-id="8cc6b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc6b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8cc6b-133">displayName</span></span>|<span data-ttu-id="8cc6b-134">String</span><span class="sxs-lookup"><span data-stu-id="8cc6b-134">String</span></span>|<span data-ttu-id="8cc6b-135">Имя тега.</span><span class="sxs-lookup"><span data-stu-id="8cc6b-135">Name of the tag.</span></span> <span data-ttu-id="8cc6b-136">Значение не может быть больше 40 символов.</span><span class="sxs-lookup"><span data-stu-id="8cc6b-136">The value can't be more than 40 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="8cc6b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cc6b-137">Response</span></span>

<span data-ttu-id="8cc6b-138">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [teamworkTag](../resources/teamworktag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8cc6b-138">If successful, this method returns a `200 OK` response code and an updated [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8cc6b-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="8cc6b-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8cc6b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cc6b-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8cc6b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc6b-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamworktag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
Content-Type: application/json
Content-length: 185

{
  "displayName": "Finance"
}
```
# <a name="c"></a>[<span data-ttu-id="8cc6b-142">C#</span><span class="sxs-lookup"><span data-stu-id="8cc6b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-teamworktag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cc6b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cc6b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamworktag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cc6b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cc6b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-teamworktag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cc6b-145">Java</span><span class="sxs-lookup"><span data-stu-id="8cc6b-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-teamworktag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8cc6b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cc6b-146">Response</span></span>
><span data-ttu-id="8cc6b-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8cc6b-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Finance",
  "memberCount": 2,
  "tagType": "standard"
}
```
