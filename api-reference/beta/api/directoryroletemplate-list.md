---
title: Список объектов directoryRoleTemplate
description: Получение списка объектов directoryroletemplate.
ms.openlocfilehash: 58d88187c7b7791ca0b4308fdd6224c6bebc4a8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075270"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="5614b-103">Список объектов directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="5614b-103">List directoryRoleTemplates</span></span>

> <span data-ttu-id="5614b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5614b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5614b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5614b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5614b-106">Получение списка объектов directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="5614b-106">Retrieve a list of directoryroletemplate objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5614b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5614b-107">Permissions</span></span>
<span data-ttu-id="5614b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5614b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5614b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5614b-110">Permission type</span></span>      | <span data-ttu-id="5614b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5614b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5614b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5614b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5614b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5614b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5614b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5614b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5614b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5614b-115">Not supported.</span></span>    |
|<span data-ttu-id="5614b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5614b-116">Application</span></span> | <span data-ttu-id="5614b-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5614b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5614b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5614b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5614b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5614b-119">Optional query parameters</span></span>
<span data-ttu-id="5614b-120">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="5614b-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5614b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5614b-121">Request headers</span></span>
| <span data-ttu-id="5614b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5614b-122">Name</span></span>       | <span data-ttu-id="5614b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5614b-123">Type</span></span> | <span data-ttu-id="5614b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5614b-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5614b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5614b-125">Authorization</span></span>  | <span data-ttu-id="5614b-126">string</span><span class="sxs-lookup"><span data-stu-id="5614b-126">string</span></span>  | <span data-ttu-id="5614b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5614b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5614b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5614b-129">Request body</span></span>
<span data-ttu-id="5614b-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5614b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5614b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5614b-131">Response</span></span>

<span data-ttu-id="5614b-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5614b-132">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5614b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5614b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5614b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5614b-134">Request</span></span>
<span data-ttu-id="5614b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5614b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="5614b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5614b-136">Response</span></span>
<span data-ttu-id="5614b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5614b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 139

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
