---
title: ОтКлонить riskyUsers
description: Отклонение риска для объекта riskyUsers.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 3027320b25c35e60e1b5dccabc7ff34ea642a953
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537786"
---
# <a name="dismiss-riskyusers"></a><span data-ttu-id="99c87-103">ОтКлонить riskyUsers</span><span class="sxs-lookup"><span data-stu-id="99c87-103">Dismiss riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="99c87-104">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="99c87-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="99c87-105">Отклонение риска для объекта **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="99c87-105">Dismiss the risk of a **riskyUser** object.</span></span> <span data-ttu-id="99c87-106">Это действие установит для уровня риска целевого пользователя значение нет.</span><span class="sxs-lookup"><span data-stu-id="99c87-106">This action will set the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="99c87-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99c87-107">Permissions</span></span>
<span data-ttu-id="99c87-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99c87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99c87-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99c87-110">Permission type</span></span>      | <span data-ttu-id="99c87-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99c87-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99c87-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99c87-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99c87-113">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="99c87-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="99c87-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99c87-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99c87-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99c87-115">Not supported.</span></span>    |
|<span data-ttu-id="99c87-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99c87-116">Application</span></span> | <span data-ttu-id="99c87-117">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="99c87-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99c87-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99c87-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="99c87-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99c87-119">Request headers</span></span>
| <span data-ttu-id="99c87-120">Имя</span><span class="sxs-lookup"><span data-stu-id="99c87-120">Name</span></span>      |<span data-ttu-id="99c87-121">Описание</span><span class="sxs-lookup"><span data-stu-id="99c87-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99c87-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99c87-122">Authorization</span></span>  | <span data-ttu-id="99c87-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99c87-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99c87-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="99c87-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="99c87-126">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="99c87-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="99c87-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="99c87-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99c87-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99c87-128">Request body</span></span>
<span data-ttu-id="99c87-129">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="99c87-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="99c87-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="99c87-130">Response</span></span>

<span data-ttu-id="99c87-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99c87-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99c87-133">Пример</span><span class="sxs-lookup"><span data-stu-id="99c87-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99c87-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="99c87-134">Request</span></span>
<span data-ttu-id="99c87-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99c87-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="99c87-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="99c87-136">Response</span></span>
<span data-ttu-id="99c87-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="99c87-137">Here is an example of the response.</span></span>
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
