---
title: Создание объекта ContactFolder
description: 'Создание дочернего объекта contactFolder указанной папки. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 66061d86b3c3894c165788cd408b22b8824b34f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991771"
---
# <a name="create-contactfolder"></a><span data-ttu-id="e5608-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="e5608-103">Create ContactFolder</span></span>

> <span data-ttu-id="e5608-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5608-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5608-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5608-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5608-106">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="e5608-106">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="e5608-107">Вы также можете [создать объект contactFolder в папке контактов пользователя по умолчанию](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="e5608-107">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e5608-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5608-108">Permissions</span></span>
<span data-ttu-id="e5608-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5608-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5608-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5608-111">Permission type</span></span>      | <span data-ttu-id="e5608-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5608-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5608-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5608-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e5608-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5608-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e5608-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5608-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5608-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5608-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e5608-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5608-117">Application</span></span> | <span data-ttu-id="e5608-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5608-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5608-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5608-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="e5608-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5608-120">Request headers</span></span>
| <span data-ttu-id="e5608-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5608-121">Header</span></span>       | <span data-ttu-id="e5608-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5608-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5608-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5608-123">Authorization</span></span>  | <span data-ttu-id="e5608-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5608-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e5608-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5608-126">Content-Type</span></span>  | <span data-ttu-id="e5608-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5608-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5608-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5608-129">Request body</span></span>
<span data-ttu-id="e5608-130">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5608-130">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e5608-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5608-131">Response</span></span>

<span data-ttu-id="e5608-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5608-132">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5608-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e5608-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5608-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5608-134">Request</span></span>
<span data-ttu-id="e5608-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5608-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="e5608-136">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5608-136">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e5608-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5608-137">Response</span></span>
<span data-ttu-id="e5608-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5608-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
