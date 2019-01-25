---
title: Перечисление категорий Outlook
description: Получение всех категорий, определенных для пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5a375079748be356b37cb2281f10da857cca2563
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523605"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="ba116-103">Перечисление категорий Outlook</span><span class="sxs-lookup"><span data-stu-id="ba116-103">List Outlook categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba116-104">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba116-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba116-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba116-105">Permissions</span></span>
<span data-ttu-id="ba116-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba116-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba116-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba116-108">Permission type</span></span>      | <span data-ttu-id="ba116-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba116-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba116-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba116-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba116-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ba116-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ba116-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba116-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba116-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ba116-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ba116-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba116-114">Application</span></span> | <span data-ttu-id="ba116-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ba116-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba116-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba116-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ba116-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba116-117">Optional query parameters</span></span>
<span data-ttu-id="ba116-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ba116-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba116-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba116-119">Request headers</span></span>
| <span data-ttu-id="ba116-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ba116-120">Name</span></span>      |<span data-ttu-id="ba116-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ba116-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba116-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba116-122">Authorization</span></span>  | <span data-ttu-id="ba116-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba116-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba116-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba116-125">Request body</span></span>
<span data-ttu-id="ba116-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba116-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba116-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba116-127">Response</span></span>

<span data-ttu-id="ba116-128">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ba116-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba116-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ba116-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba116-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba116-130">Request</span></span>
<span data-ttu-id="ba116-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba116-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories
```
##### <a name="response"></a><span data-ttu-id="ba116-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba116-132">Response</span></span>
<span data-ttu-id="ba116-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ba116-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-mastercategories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
