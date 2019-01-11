---
title: Создание объекта ContactFolder
description: 'Создание дочернего объекта contactFolder указанной папки. '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 879c0b642a9db22184617544f9cb9be4a7d29cce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836297"
---
# <a name="create-contactfolder"></a><span data-ttu-id="498e8-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="498e8-103">Create ContactFolder</span></span>

<span data-ttu-id="498e8-104">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="498e8-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="498e8-105">Вы также можете [создать объект contactFolder в папке контактов пользователя по умолчанию](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="498e8-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="498e8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="498e8-106">Permissions</span></span>
<span data-ttu-id="498e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="498e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="498e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="498e8-109">Permission type</span></span>      | <span data-ttu-id="498e8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="498e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="498e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="498e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="498e8-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="498e8-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="498e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="498e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="498e8-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="498e8-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="498e8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="498e8-115">Application</span></span> | <span data-ttu-id="498e8-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="498e8-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="498e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="498e8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="498e8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="498e8-118">Request headers</span></span>
| <span data-ttu-id="498e8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="498e8-119">Header</span></span>       | <span data-ttu-id="498e8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="498e8-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="498e8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="498e8-121">Authorization</span></span>  | <span data-ttu-id="498e8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="498e8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="498e8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="498e8-124">Content-Type</span></span>  | <span data-ttu-id="498e8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="498e8-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="498e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="498e8-127">Request body</span></span>
<span data-ttu-id="498e8-128">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="498e8-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="498e8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="498e8-129">Response</span></span>

<span data-ttu-id="498e8-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="498e8-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="498e8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="498e8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="498e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="498e8-132">Request</span></span>
<span data-ttu-id="498e8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="498e8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="498e8-134">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="498e8-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="498e8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="498e8-135">Response</span></span>
<span data-ttu-id="498e8-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="498e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
