---
title: Создание объекта ContactFolder
description: Создание объекта contactFolder в стандартной папке контактов пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 75550f7468bda678d20f09343a7150d5f4e70fd7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521903"
---
# <a name="create-contactfolder"></a><span data-ttu-id="97a75-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="97a75-103">Create ContactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a75-104">Создание объекта contactFolder в стандартной папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="97a75-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="97a75-105">Вы также можете [создать экземпляр contactfolder в качестве дочернего для любой указанной папки контактов](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="97a75-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="97a75-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97a75-106">Permissions</span></span>
<span data-ttu-id="97a75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97a75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97a75-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97a75-109">Permission type</span></span>      | <span data-ttu-id="97a75-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97a75-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97a75-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97a75-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97a75-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97a75-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="97a75-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97a75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97a75-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97a75-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="97a75-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97a75-115">Application</span></span> | <span data-ttu-id="97a75-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97a75-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="97a75-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97a75-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="97a75-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97a75-118">Request headers</span></span>
| <span data-ttu-id="97a75-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97a75-119">Header</span></span>       | <span data-ttu-id="97a75-120">Значение</span><span class="sxs-lookup"><span data-stu-id="97a75-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97a75-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97a75-121">Authorization</span></span>  | <span data-ttu-id="97a75-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97a75-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97a75-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97a75-124">Content-Type</span></span>  | <span data-ttu-id="97a75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97a75-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97a75-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97a75-126">Request body</span></span>
<span data-ttu-id="97a75-127">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97a75-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="97a75-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="97a75-128">Response</span></span>

<span data-ttu-id="97a75-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97a75-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97a75-130">Пример</span><span class="sxs-lookup"><span data-stu-id="97a75-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97a75-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="97a75-131">Request</span></span>
<span data-ttu-id="97a75-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97a75-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="97a75-133">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97a75-133">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="97a75-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="97a75-134">Response</span></span>
<span data-ttu-id="97a75-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="97a75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-contactfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
