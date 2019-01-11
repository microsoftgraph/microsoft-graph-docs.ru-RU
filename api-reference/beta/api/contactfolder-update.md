---
title: Обновление объекта contactFolder
description: Обновление свойств объекта contactfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 155a8fb17f0423e2a4718dde8fc9743d8c1f0342
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854763"
---
# <a name="update-contactfolder"></a><span data-ttu-id="48746-103">Обновление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="48746-103">Update contactfolder</span></span>

> <span data-ttu-id="48746-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48746-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48746-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48746-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48746-106">Обновление свойств объекта contactfolder.</span><span class="sxs-lookup"><span data-stu-id="48746-106">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="48746-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48746-107">Permissions</span></span>
<span data-ttu-id="48746-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48746-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48746-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48746-110">Permission type</span></span>      | <span data-ttu-id="48746-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48746-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48746-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48746-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48746-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48746-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="48746-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48746-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48746-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48746-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="48746-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48746-116">Application</span></span> | <span data-ttu-id="48746-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48746-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="48746-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48746-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="48746-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48746-119">Request headers</span></span>
| <span data-ttu-id="48746-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48746-120">Header</span></span>       | <span data-ttu-id="48746-121">Значение</span><span class="sxs-lookup"><span data-stu-id="48746-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48746-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48746-122">Authorization</span></span>  | <span data-ttu-id="48746-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48746-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48746-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48746-125">Content-Type</span></span>  | <span data-ttu-id="48746-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48746-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48746-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48746-128">Request body</span></span>
<span data-ttu-id="48746-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="48746-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="48746-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="48746-132">Property</span></span>     | <span data-ttu-id="48746-133">Тип</span><span class="sxs-lookup"><span data-stu-id="48746-133">Type</span></span>   |<span data-ttu-id="48746-134">Описание</span><span class="sxs-lookup"><span data-stu-id="48746-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48746-135">displayName</span><span class="sxs-lookup"><span data-stu-id="48746-135">displayName</span></span>|<span data-ttu-id="48746-136">String</span><span class="sxs-lookup"><span data-stu-id="48746-136">String</span></span>|<span data-ttu-id="48746-137">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="48746-137">The folder's display name.</span></span>|
|<span data-ttu-id="48746-138">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="48746-138">parentFolderId</span></span>|<span data-ttu-id="48746-139">String</span><span class="sxs-lookup"><span data-stu-id="48746-139">String</span></span>|<span data-ttu-id="48746-140">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="48746-140">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="48746-141">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="48746-141">wellKnownName</span></span>|<span data-ttu-id="48746-142">string</span><span class="sxs-lookup"><span data-stu-id="48746-142">string</span></span>|<span data-ttu-id="48746-143">Имя папки, если распознанный папки.</span><span class="sxs-lookup"><span data-stu-id="48746-143">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="48746-144">В настоящее время `contacts` является единственным папку распознанный контакты.</span><span class="sxs-lookup"><span data-stu-id="48746-144">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="48746-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="48746-145">Response</span></span>

<span data-ttu-id="48746-146">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48746-146">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48746-147">Пример</span><span class="sxs-lookup"><span data-stu-id="48746-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48746-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="48746-148">Request</span></span>
<span data-ttu-id="48746-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48746-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="48746-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="48746-150">Response</span></span>
<span data-ttu-id="48746-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48746-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "wellKnownName": "wellKnownName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
