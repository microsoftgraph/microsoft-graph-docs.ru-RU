---
title: Создание категории Outlook
description: Создание объекта outlookCategory в основном списке категорий пользователя.
localization_priority: Normal
ms.openlocfilehash: 4f032bff358fbc3c07b30f925abee27664c01c8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807093"
---
# <a name="create-outlook-category"></a><span data-ttu-id="3558c-103">Создание категории Outlook</span><span class="sxs-lookup"><span data-stu-id="3558c-103">Create Outlook category</span></span>

> <span data-ttu-id="3558c-104">**Важно**: интерфейсы API в разделе версии /beta в Microsoft Graph в предварительной версии и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3558c-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3558c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3558c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3558c-106">Создание объекта [outlookCategory](../resources/outlookcategory.md) в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="3558c-106">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="3558c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3558c-107">Permissions</span></span>
<span data-ttu-id="3558c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3558c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3558c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3558c-110">Permission type</span></span>      | <span data-ttu-id="3558c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3558c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3558c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3558c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3558c-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3558c-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3558c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3558c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3558c-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3558c-115">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="3558c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3558c-116">Application</span></span> | <span data-ttu-id="3558c-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3558c-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3558c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3558c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="3558c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3558c-119">Request headers</span></span>
| <span data-ttu-id="3558c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3558c-120">Name</span></span>       | <span data-ttu-id="3558c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3558c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3558c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3558c-122">Authorization</span></span>  | <span data-ttu-id="3558c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3558c-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3558c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3558c-125">Request body</span></span>
<span data-ttu-id="3558c-126">Включите в текст запроса описание объекта [outlookCategory](../resources/outlookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3558c-126">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3558c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3558c-127">Response</span></span>

<span data-ttu-id="3558c-128">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и новый объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3558c-128">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3558c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3558c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3558c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3558c-130">Request</span></span>
<span data-ttu-id="3558c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3558c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="3558c-132">Включите в текст запроса описание объекта [outlookCategory](../resources/outlookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3558c-132">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3558c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="3558c-133">Response</span></span>
<span data-ttu-id="3558c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3558c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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
