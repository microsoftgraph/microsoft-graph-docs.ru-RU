---
title: Создание объекта MailFolder
description: С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.
localization_priority: Normal
ms.openlocfilehash: fd625e221eea67d08407dc332d47880ce21f21e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838425"
---
# <a name="create-mailfolder"></a><span data-ttu-id="02b4b-103">Создание объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="02b4b-103">Create MailFolder</span></span>

> <span data-ttu-id="02b4b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02b4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02b4b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02b4b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02b4b-106">С помощью этого API можно создать папку почты в корневой папке почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="02b4b-106">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="02b4b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02b4b-107">Permissions</span></span>
<span data-ttu-id="02b4b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02b4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02b4b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02b4b-110">Permission type</span></span>      | <span data-ttu-id="02b4b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02b4b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02b4b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02b4b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02b4b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02b4b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="02b4b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02b4b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02b4b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02b4b-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="02b4b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02b4b-116">Application</span></span> | <span data-ttu-id="02b4b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02b4b-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="02b4b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02b4b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="02b4b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02b4b-119">Request headers</span></span>
| <span data-ttu-id="02b4b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02b4b-120">Header</span></span>       | <span data-ttu-id="02b4b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="02b4b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02b4b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02b4b-122">Authorization</span></span>  | <span data-ttu-id="02b4b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02b4b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="02b4b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02b4b-125">Content-Type</span></span>  | <span data-ttu-id="02b4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02b4b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02b4b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02b4b-127">Request body</span></span>
<span data-ttu-id="02b4b-p104">Предоставьте в тексте запроса объект JSON с указанными ниже параметрами. **displayName** — это единственное доступное для записи свойство объекта [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="02b4b-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="02b4b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="02b4b-130">Parameter</span></span>    | <span data-ttu-id="02b4b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="02b4b-131">Type</span></span>   |<span data-ttu-id="02b4b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="02b4b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02b4b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="02b4b-133">displayName</span></span>|<span data-ttu-id="02b4b-134">String</span><span class="sxs-lookup"><span data-stu-id="02b4b-134">String</span></span>|<span data-ttu-id="02b4b-135">Отображаемое имя новой папки.</span><span class="sxs-lookup"><span data-stu-id="02b4b-135">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="02b4b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="02b4b-136">Response</span></span>

<span data-ttu-id="02b4b-137">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [MailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="02b4b-137">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02b4b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="02b4b-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02b4b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="02b4b-139">Request</span></span>
<span data-ttu-id="02b4b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02b4b-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="02b4b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="02b4b-141">Response</span></span>
<span data-ttu-id="02b4b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="02b4b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
