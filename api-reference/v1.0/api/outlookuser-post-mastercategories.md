---
title: Создание категории Outlook
description: Создание объекта outlookCategory в основном списке категорий пользователя.
localization_priority: Normal
ms.openlocfilehash: 71bb00d96119b06fda624b02fa9b64be67313f6e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815381"
---
# <a name="create-outlook-category"></a><span data-ttu-id="15ea8-103">Создание категории Outlook</span><span class="sxs-lookup"><span data-stu-id="15ea8-103">Create Outlook category</span></span>


<span data-ttu-id="15ea8-104">Создание объекта [outlookCategory](../resources/outlookcategory.md) в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="15ea8-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="15ea8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15ea8-105">Permissions</span></span>
<span data-ttu-id="15ea8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15ea8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15ea8-108">Permission type</span></span>      | <span data-ttu-id="15ea8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15ea8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15ea8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15ea8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15ea8-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ea8-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="15ea8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15ea8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ea8-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ea8-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="15ea8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15ea8-114">Application</span></span> | <span data-ttu-id="15ea8-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ea8-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="15ea8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15ea8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="15ea8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15ea8-117">Request headers</span></span>
| <span data-ttu-id="15ea8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="15ea8-118">Name</span></span>       | <span data-ttu-id="15ea8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="15ea8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="15ea8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15ea8-120">Authorization</span></span>  | <span data-ttu-id="15ea8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15ea8-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="15ea8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15ea8-123">Request body</span></span>
<span data-ttu-id="15ea8-124">Включите в текст запроса описание объекта [outlookCategory](../resources/outlookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15ea8-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="15ea8-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="15ea8-125">Response</span></span>

<span data-ttu-id="15ea8-126">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и новый объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="15ea8-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15ea8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="15ea8-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15ea8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="15ea8-128">Request</span></span>
<span data-ttu-id="15ea8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15ea8-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="15ea8-130">Включите в текст запроса описание объекта [outlookCategory](../resources/outlookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15ea8-130">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="15ea8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="15ea8-131">Response</span></span>
<span data-ttu-id="15ea8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="15ea8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
