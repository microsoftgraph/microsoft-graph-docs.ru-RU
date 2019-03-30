---
title: Подтверждение riskyUsers скомпрометированных атак
description: Подтвердите, что объект riskyUsers скомпрометирован.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 9ae07bf8d1d4a41764aa145a9c7508da339d7ce2
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2019
ms.locfileid: "31013126"
---
# <a name="confirm-riskyusers-compromised"></a><span data-ttu-id="94cd9-103">Подтверждение riskyUsers скомпрометированных атак</span><span class="sxs-lookup"><span data-stu-id="94cd9-103">Confirm riskyUsers compromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="94cd9-104">**Примечание:** Для API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="94cd9-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="94cd9-105">Подтвердите, что объект [riskyUsers](../resources/riskyuser.md) скомпрометирован.</span><span class="sxs-lookup"><span data-stu-id="94cd9-105">Confirm a [riskyUsers](../resources/riskyuser.md) object as compromised.</span></span> <span data-ttu-id="94cd9-106">При этом уровень риска целевого пользователя будет установлен в значение High (высокий).</span><span class="sxs-lookup"><span data-stu-id="94cd9-106">This will set the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="94cd9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94cd9-107">Permissions</span></span>
<span data-ttu-id="94cd9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94cd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94cd9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94cd9-110">Permission type</span></span>      | <span data-ttu-id="94cd9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94cd9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94cd9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94cd9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94cd9-113">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="94cd9-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="94cd9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94cd9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94cd9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94cd9-115">Not supported.</span></span>    |
|<span data-ttu-id="94cd9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94cd9-116">Application</span></span> | <span data-ttu-id="94cd9-117">Идентитирискюсер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="94cd9-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94cd9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94cd9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="94cd9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94cd9-119">Request headers</span></span>
| <span data-ttu-id="94cd9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="94cd9-120">Name</span></span>      |<span data-ttu-id="94cd9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="94cd9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94cd9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94cd9-122">Authorization</span></span>  | <span data-ttu-id="94cd9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94cd9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94cd9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="94cd9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="94cd9-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="94cd9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94cd9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94cd9-128">Request body</span></span>
<span data-ttu-id="94cd9-129">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="94cd9-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="94cd9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="94cd9-130">Response</span></span>

<span data-ttu-id="94cd9-131">В случае успеха этот метод возвращает код `204 No Content` отклика</span><span class="sxs-lookup"><span data-stu-id="94cd9-131">If successful, this method returns a `204 No Content` response code</span></span>
## <a name="example"></a><span data-ttu-id="94cd9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="94cd9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94cd9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="94cd9-133">Request</span></span>
<span data-ttu-id="94cd9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94cd9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised


Request Body
{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="94cd9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="94cd9-135">Response</span></span>
<span data-ttu-id="94cd9-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="94cd9-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 204 NoContent
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
