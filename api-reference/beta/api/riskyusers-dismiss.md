---
title: ОтКлонить riskyUsers
description: Отклонение риска для объекта riskyUsers.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 3027320b25c35e60e1b5dccabc7ff34ea642a953
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2019
ms.locfileid: "31560103"
---
# <a name="dismiss-riskyusers"></a><span data-ttu-id="d339c-103">ОтКлонить riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d339c-103">Dismiss riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="d339c-104">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="d339c-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="d339c-105">Отклонение риска для объекта **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="d339c-105">Dismiss the risk of a **riskyUser** object.</span></span> <span data-ttu-id="d339c-106">Это действие установит для уровня риска целевого пользователя значение нет.</span><span class="sxs-lookup"><span data-stu-id="d339c-106">This action will set the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="d339c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d339c-107">Permissions</span></span>
<span data-ttu-id="d339c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d339c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d339c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d339c-110">Permission type</span></span>      | <span data-ttu-id="d339c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d339c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d339c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d339c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d339c-113">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d339c-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="d339c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d339c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d339c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d339c-115">Not supported.</span></span>    |
|<span data-ttu-id="d339c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d339c-116">Application</span></span> | <span data-ttu-id="d339c-117">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d339c-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d339c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d339c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="d339c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d339c-119">Request headers</span></span>
| <span data-ttu-id="d339c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d339c-120">Name</span></span>      |<span data-ttu-id="d339c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d339c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d339c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d339c-122">Authorization</span></span>  | <span data-ttu-id="d339c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d339c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d339c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d339c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d339c-126">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="d339c-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="d339c-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d339c-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d339c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d339c-128">Request body</span></span>
<span data-ttu-id="d339c-129">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="d339c-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="d339c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d339c-130">Response</span></span>

<span data-ttu-id="d339c-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d339c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d339c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d339c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d339c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d339c-134">Request</span></span>
<span data-ttu-id="d339c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d339c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="d339c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d339c-136">Response</span></span>
<span data-ttu-id="d339c-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d339c-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
