---
title: Создание объекта ContactFolder
description: 'Создание дочернего объекта contactFolder указанной папки. '
author: angelgolfer-ms
ms.openlocfilehash: a6b638610ed487fe69d80254c36efc3478f476cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336486"
---
# <a name="create-contactfolder"></a><span data-ttu-id="5e457-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="5e457-103">Create ContactFolder</span></span>

> <span data-ttu-id="5e457-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e457-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e457-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e457-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e457-106">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="5e457-106">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="5e457-107">Вы также можете [создать объект contactFolder в папке контактов пользователя по умолчанию](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="5e457-107">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5e457-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e457-108">Permissions</span></span>
<span data-ttu-id="5e457-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e457-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e457-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e457-111">Permission type</span></span>      | <span data-ttu-id="5e457-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e457-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e457-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e457-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5e457-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e457-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5e457-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e457-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e457-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e457-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5e457-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e457-117">Application</span></span> | <span data-ttu-id="5e457-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e457-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e457-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e457-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="5e457-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e457-120">Request headers</span></span>
| <span data-ttu-id="5e457-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e457-121">Header</span></span>       | <span data-ttu-id="5e457-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e457-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e457-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e457-123">Authorization</span></span>  | <span data-ttu-id="5e457-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e457-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e457-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e457-126">Content-Type</span></span>  | <span data-ttu-id="5e457-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e457-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e457-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e457-129">Request body</span></span>
<span data-ttu-id="5e457-130">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e457-130">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5e457-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e457-131">Response</span></span>

<span data-ttu-id="5e457-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e457-132">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e457-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5e457-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e457-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e457-134">Request</span></span>
<span data-ttu-id="5e457-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e457-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="5e457-136">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e457-136">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5e457-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e457-137">Response</span></span>
<span data-ttu-id="5e457-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e457-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
