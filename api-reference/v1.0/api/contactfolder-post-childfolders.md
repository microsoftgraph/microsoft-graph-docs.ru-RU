---
title: Создание объекта ContactFolder
description: 'Создание дочернего объекта contactFolder указанной папки. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f7cd5d35bce0e23fcc10f88dde524d3e80faebf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566201"
---
# <a name="create-contactfolder"></a><span data-ttu-id="ae47f-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="ae47f-103">Create ContactFolder</span></span>

<span data-ttu-id="ae47f-104">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="ae47f-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="ae47f-105">Вы также можете [создать объект contactFolder в папке контактов пользователя по умолчанию](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="ae47f-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ae47f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae47f-106">Permissions</span></span>
<span data-ttu-id="ae47f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae47f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae47f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae47f-109">Permission type</span></span>      | <span data-ttu-id="ae47f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae47f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae47f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae47f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae47f-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae47f-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ae47f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae47f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae47f-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae47f-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ae47f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae47f-115">Application</span></span> | <span data-ttu-id="ae47f-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae47f-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae47f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae47f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="ae47f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae47f-118">Request headers</span></span>
| <span data-ttu-id="ae47f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae47f-119">Header</span></span>       | <span data-ttu-id="ae47f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ae47f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae47f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae47f-121">Authorization</span></span>  | <span data-ttu-id="ae47f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae47f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ae47f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae47f-124">Content-Type</span></span>  | <span data-ttu-id="ae47f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae47f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae47f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae47f-127">Request body</span></span>
<span data-ttu-id="ae47f-128">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae47f-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae47f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae47f-129">Response</span></span>

<span data-ttu-id="ae47f-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae47f-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae47f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ae47f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae47f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae47f-132">Request</span></span>
<span data-ttu-id="ae47f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae47f-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="ae47f-134">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae47f-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ae47f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae47f-135">Response</span></span>
<span data-ttu-id="ae47f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae47f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
