---
title: Создание объекта ContactFolder
description: Создание объекта contactFolder в стандартной папке контактов пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b9cf3dfb855b261b47e1a5614eda7602a50a363
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953569"
---
# <a name="create-contactfolder"></a><span data-ttu-id="28731-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="28731-103">Create ContactFolder</span></span>

> <span data-ttu-id="28731-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="28731-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28731-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28731-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28731-106">Создание объекта contactFolder в стандартной папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="28731-106">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="28731-107">Вы также можете [создать экземпляр contactfolder в качестве дочернего для любой указанной папки контактов](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="28731-107">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="28731-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28731-108">Permissions</span></span>
<span data-ttu-id="28731-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28731-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28731-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28731-111">Permission type</span></span>      | <span data-ttu-id="28731-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28731-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28731-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28731-113">Delegated (work or school account)</span></span> | <span data-ttu-id="28731-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28731-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="28731-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28731-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28731-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28731-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="28731-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28731-117">Application</span></span> | <span data-ttu-id="28731-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28731-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="28731-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28731-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="28731-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28731-120">Request headers</span></span>
| <span data-ttu-id="28731-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28731-121">Header</span></span>       | <span data-ttu-id="28731-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28731-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28731-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28731-123">Authorization</span></span>  | <span data-ttu-id="28731-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28731-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="28731-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28731-126">Content-Type</span></span>  | <span data-ttu-id="28731-127">application/json</span><span class="sxs-lookup"><span data-stu-id="28731-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28731-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28731-128">Request body</span></span>
<span data-ttu-id="28731-129">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28731-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="28731-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="28731-130">Response</span></span>

<span data-ttu-id="28731-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28731-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28731-132">Пример</span><span class="sxs-lookup"><span data-stu-id="28731-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28731-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="28731-133">Request</span></span>
<span data-ttu-id="28731-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28731-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="28731-135">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28731-135">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="28731-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="28731-136">Response</span></span>
<span data-ttu-id="28731-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="28731-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
