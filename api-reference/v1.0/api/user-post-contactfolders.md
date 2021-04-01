---
title: Создание объекта ContactFolder
description: Создание объекта contactFolder в стандартной папке контактов пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 76f7f7592657e913322343426c07575344fc4d68
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473551"
---
# <a name="create-contactfolder"></a><span data-ttu-id="62832-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="62832-103">Create ContactFolder</span></span>

<span data-ttu-id="62832-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62832-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62832-105">Создание объекта contactFolder в стандартной папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="62832-105">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="62832-106">Вы также можете [создать экземпляр contactfolder в качестве дочернего для любой указанной папки контактов](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="62832-106">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="62832-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62832-107">Permissions</span></span>
<span data-ttu-id="62832-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62832-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62832-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62832-110">Permission type</span></span>      | <span data-ttu-id="62832-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62832-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62832-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62832-112">Delegated (work or school account)</span></span> | <span data-ttu-id="62832-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62832-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="62832-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62832-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62832-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62832-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="62832-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62832-116">Application</span></span> | <span data-ttu-id="62832-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62832-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="62832-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62832-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="62832-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62832-119">Request headers</span></span>
| <span data-ttu-id="62832-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62832-120">Header</span></span>       | <span data-ttu-id="62832-121">Значение</span><span class="sxs-lookup"><span data-stu-id="62832-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="62832-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62832-122">Authorization</span></span>  | <span data-ttu-id="62832-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62832-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="62832-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62832-125">Content-Type</span></span>  | <span data-ttu-id="62832-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62832-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62832-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62832-127">Request body</span></span>
<span data-ttu-id="62832-128">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62832-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="62832-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="62832-129">Response</span></span>

<span data-ttu-id="62832-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62832-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62832-131">Пример</span><span class="sxs-lookup"><span data-stu-id="62832-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="62832-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="62832-132">Request</span></span>
<span data-ttu-id="62832-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62832-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Important contacts"
}
```

<span data-ttu-id="62832-134">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62832-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="62832-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="62832-135">Response</span></span>
<span data-ttu-id="62832-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62832-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Important contacts",
  "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy04MDU0LTBkOTFkY2Y5NzE1NAAuAAAAAADESc12GiymT5Zp9IHtHnWZAQA2t6otiDF0TYOkcEEh3vhfAAAGgUC1AAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

