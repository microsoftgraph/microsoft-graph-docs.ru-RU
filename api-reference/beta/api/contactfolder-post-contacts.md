---
title: Создание объекта Contact
description: Добавление контакта в корневую папку контактов или в конечную точку `contacts` другой папки контактов.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3fd45ee7f77e2d485b7a972b8454807368796226
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528062"
---
# <a name="create-contact"></a><span data-ttu-id="0cf63-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="0cf63-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cf63-104">Добавление контакта в корневую папку контактов или в конечную точку `contacts` другой папки контактов.</span><span class="sxs-lookup"><span data-stu-id="0cf63-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="0cf63-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cf63-105">Permissions</span></span>
<span data-ttu-id="0cf63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cf63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cf63-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cf63-108">Permission type</span></span>      | <span data-ttu-id="0cf63-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cf63-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cf63-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cf63-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0cf63-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cf63-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0cf63-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cf63-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cf63-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cf63-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0cf63-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cf63-114">Application</span></span> | <span data-ttu-id="0cf63-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cf63-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cf63-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cf63-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="0cf63-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cf63-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="0cf63-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cf63-118">Request headers</span></span>
| <span data-ttu-id="0cf63-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cf63-119">Header</span></span>       | <span data-ttu-id="0cf63-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0cf63-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0cf63-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cf63-121">Authorization</span></span>  | <span data-ttu-id="0cf63-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cf63-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0cf63-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cf63-124">Content-Type</span></span>  | <span data-ttu-id="0cf63-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cf63-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0cf63-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cf63-127">Request body</span></span>
<span data-ttu-id="0cf63-128">Предоставьте в тексте запроса описание объекта [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cf63-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0cf63-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cf63-129">Response</span></span>

<span data-ttu-id="0cf63-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cf63-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cf63-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0cf63-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cf63-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cf63-132">Request</span></span>
<span data-ttu-id="0cf63-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cf63-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
<span data-ttu-id="0cf63-134">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cf63-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0cf63-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="0cf63-135">Response</span></span>
<span data-ttu-id="0cf63-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0cf63-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-post-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
