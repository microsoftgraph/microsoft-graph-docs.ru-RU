---
title: Создание объекта ContactFolder
description: 'Создание дочернего объекта contactFolder указанной папки. '
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4dea9aedecdacf6aff8e939a44d837d30928357b
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473250"
---
# <a name="create-contactfolder"></a><span data-ttu-id="8113f-103">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="8113f-103">Create ContactFolder</span></span>

<span data-ttu-id="8113f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8113f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8113f-105">Создание дочернего объекта contactFolder указанной папки.</span><span class="sxs-lookup"><span data-stu-id="8113f-105">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="8113f-106">Вы также можете [создать объект contactFolder в папке контактов пользователя по умолчанию](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="8113f-106">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8113f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8113f-107">Permissions</span></span>
<span data-ttu-id="8113f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8113f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8113f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8113f-110">Permission type</span></span>      | <span data-ttu-id="8113f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8113f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8113f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8113f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8113f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8113f-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8113f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8113f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8113f-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8113f-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8113f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8113f-116">Application</span></span> | <span data-ttu-id="8113f-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8113f-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8113f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8113f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="8113f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8113f-119">Request headers</span></span>
| <span data-ttu-id="8113f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8113f-120">Header</span></span>       | <span data-ttu-id="8113f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8113f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8113f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8113f-122">Authorization</span></span>  | <span data-ttu-id="8113f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8113f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8113f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8113f-125">Content-Type</span></span>  | <span data-ttu-id="8113f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8113f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8113f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8113f-128">Request body</span></span>
<span data-ttu-id="8113f-129">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8113f-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8113f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8113f-130">Response</span></span>

<span data-ttu-id="8113f-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8113f-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8113f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8113f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8113f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8113f-133">Request</span></span>

<span data-ttu-id="8113f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8113f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json

{
  "displayName": "Family"
}
```

<span data-ttu-id="8113f-135">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8113f-135">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="8113f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8113f-136">Response</span></span>

<span data-ttu-id="8113f-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8113f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Family",
  "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy04MDU0LTBkOTFkY2Y5NzE1NAAuAAAAAADESc12GiymT5Zp9IHtHnWZAQA2t6otiDF0TYOkcEEh3vhfAAAGgUC1AAA="
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
  ]
}
-->


