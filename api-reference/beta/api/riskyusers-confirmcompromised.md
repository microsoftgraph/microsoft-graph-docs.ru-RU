---
title: Подтверждение riskyUsers скомпрометированных атак
description: Подтвердите, что объект riskyUsers скомпрометирован.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: beca64415a2d03898d57cd9cda2fb248121c424b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537755"
---
# <a name="confirm-riskyusers-compromised"></a><span data-ttu-id="93d08-103">Подтверждение riskyUsers скомпрометированных атак</span><span class="sxs-lookup"><span data-stu-id="93d08-103">Confirm riskyUsers compromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="93d08-104">**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="93d08-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="93d08-105">Подтвердите, что объект [рискюсер](../resources/riskyuser.md) скомпрометирован.</span><span class="sxs-lookup"><span data-stu-id="93d08-105">Confirm a [riskyUser](../resources/riskyuser.md) object as compromised.</span></span> <span data-ttu-id="93d08-106">При этом уровень риска целевого пользователя будет установлен в значение High (высокий).</span><span class="sxs-lookup"><span data-stu-id="93d08-106">This will set the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="93d08-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93d08-107">Permissions</span></span>
<span data-ttu-id="93d08-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93d08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d08-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93d08-110">Permission type</span></span>      | <span data-ttu-id="93d08-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93d08-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d08-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93d08-112">Delegated (work or school account)</span></span> | <span data-ttu-id="93d08-113">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="93d08-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="93d08-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93d08-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93d08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93d08-115">Not supported.</span></span>    |
|<span data-ttu-id="93d08-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93d08-116">Application</span></span> | <span data-ttu-id="93d08-117">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="93d08-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93d08-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93d08-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="93d08-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93d08-119">Request headers</span></span>
| <span data-ttu-id="93d08-120">Имя</span><span class="sxs-lookup"><span data-stu-id="93d08-120">Name</span></span>      |<span data-ttu-id="93d08-121">Описание</span><span class="sxs-lookup"><span data-stu-id="93d08-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93d08-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93d08-122">Authorization</span></span>  | <span data-ttu-id="93d08-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93d08-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93d08-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="93d08-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="93d08-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="93d08-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93d08-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93d08-128">Request body</span></span>
<span data-ttu-id="93d08-129">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="93d08-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="93d08-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d08-130">Response</span></span>

<span data-ttu-id="93d08-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93d08-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93d08-133">Пример</span><span class="sxs-lookup"><span data-stu-id="93d08-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93d08-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d08-134">Request</span></span>
<span data-ttu-id="93d08-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d08-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="93d08-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d08-136">Response</span></span>
<span data-ttu-id="93d08-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93d08-137">Here is an example of the response.</span></span>
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
