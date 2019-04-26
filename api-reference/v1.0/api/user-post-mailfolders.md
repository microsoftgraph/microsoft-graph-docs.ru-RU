---
title: Создание объекта MailFolder
description: С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c2f845f2a332c7e9c7a637839727fe7b82e50a46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573594"
---
# <a name="create-mailfolder"></a><span data-ttu-id="61b7f-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="61b7f-103">Create MailFolder</span></span>

<span data-ttu-id="61b7f-104">С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="61b7f-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="61b7f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61b7f-105">Permissions</span></span>
<span data-ttu-id="61b7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61b7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61b7f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61b7f-108">Permission type</span></span>      | <span data-ttu-id="61b7f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61b7f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61b7f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61b7f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="61b7f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b7f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="61b7f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61b7f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61b7f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b7f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="61b7f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61b7f-114">Application</span></span> | <span data-ttu-id="61b7f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b7f-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="61b7f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61b7f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="61b7f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61b7f-117">Request headers</span></span>
| <span data-ttu-id="61b7f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61b7f-118">Header</span></span>       | <span data-ttu-id="61b7f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="61b7f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61b7f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61b7f-120">Authorization</span></span>  | <span data-ttu-id="61b7f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61b7f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="61b7f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61b7f-123">Content-Type</span></span>  | <span data-ttu-id="61b7f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="61b7f-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61b7f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61b7f-125">Request body</span></span>
<span data-ttu-id="61b7f-p103">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="61b7f-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="61b7f-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="61b7f-128">Parameter</span></span>    | <span data-ttu-id="61b7f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="61b7f-129">Type</span></span>   |<span data-ttu-id="61b7f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="61b7f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61b7f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="61b7f-131">displayName</span></span>|<span data-ttu-id="61b7f-132">String</span><span class="sxs-lookup"><span data-stu-id="61b7f-132">String</span></span>|<span data-ttu-id="61b7f-133">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="61b7f-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="61b7f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="61b7f-134">Response</span></span>

<span data-ttu-id="61b7f-135">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [MailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="61b7f-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61b7f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="61b7f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61b7f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="61b7f-137">Request</span></span>
<span data-ttu-id="61b7f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61b7f-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="61b7f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="61b7f-139">Response</span></span>
<span data-ttu-id="61b7f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61b7f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
