---
title: Подтверждение riskyUsers скомпрометированных атак
description: Подтвердите, что объект riskyUsers скомпрометирован.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: beca64415a2d03898d57cd9cda2fb248121c424b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336377"
---
# <a name="confirm-riskyusers-compromised"></a><span data-ttu-id="db30f-103">Подтверждение riskyUsers скомпрометированных атак</span><span class="sxs-lookup"><span data-stu-id="db30f-103">Confirm riskyUsers compromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="db30f-104">**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="db30f-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="db30f-105">Подтвердите, что объект [рискюсер](../resources/riskyuser.md) скомпрометирован.</span><span class="sxs-lookup"><span data-stu-id="db30f-105">Confirm a [riskyUser](../resources/riskyuser.md) object as compromised.</span></span> <span data-ttu-id="db30f-106">При этом уровень риска целевого пользователя будет установлен в значение High (высокий).</span><span class="sxs-lookup"><span data-stu-id="db30f-106">This will set the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="db30f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db30f-107">Permissions</span></span>
<span data-ttu-id="db30f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db30f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db30f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db30f-110">Permission type</span></span>      | <span data-ttu-id="db30f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db30f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db30f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db30f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db30f-113">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="db30f-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="db30f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db30f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db30f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db30f-115">Not supported.</span></span>    |
|<span data-ttu-id="db30f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db30f-116">Application</span></span> | <span data-ttu-id="db30f-117">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="db30f-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db30f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db30f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="db30f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db30f-119">Request headers</span></span>
| <span data-ttu-id="db30f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="db30f-120">Name</span></span>      |<span data-ttu-id="db30f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="db30f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db30f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db30f-122">Authorization</span></span>  | <span data-ttu-id="db30f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db30f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db30f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db30f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="db30f-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="db30f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db30f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db30f-128">Request body</span></span>
<span data-ttu-id="db30f-129">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="db30f-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="db30f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="db30f-130">Response</span></span>

<span data-ttu-id="db30f-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db30f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db30f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="db30f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db30f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="db30f-134">Request</span></span>
<span data-ttu-id="db30f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db30f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="db30f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db30f-136">Response</span></span>
<span data-ttu-id="db30f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db30f-137">Here is an example of the response.</span></span>
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
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
