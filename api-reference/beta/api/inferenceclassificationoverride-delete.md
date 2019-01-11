---
title: Удаление объекта inferenceClassificationOverride
description: Удалить фокус папки "Входящие" переопределение, указанный по идентификатору.
localization_priority: Normal
ms.openlocfilehash: 7db351e11ccfa8e88fe97ff1ee22173a87242d57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870142"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="c10e3-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="c10e3-103">Delete inferenceClassificationOverride</span></span>

> <span data-ttu-id="c10e3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c10e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c10e3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c10e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c10e3-106">Удалить [Фокус папки "Входящие"](../resources/manage-focused-inbox.md) переопределение, указанный по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="c10e3-106">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="c10e3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c10e3-107">Permissions</span></span>
<span data-ttu-id="c10e3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c10e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c10e3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c10e3-110">Permission type</span></span>      | <span data-ttu-id="c10e3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c10e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c10e3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c10e3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c10e3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c10e3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c10e3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c10e3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c10e3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c10e3-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c10e3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c10e3-116">Application</span></span> | <span data-ttu-id="c10e3-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c10e3-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c10e3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c10e3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c10e3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c10e3-119">Request headers</span></span>
| <span data-ttu-id="c10e3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c10e3-120">Name</span></span>       | <span data-ttu-id="c10e3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c10e3-121">Type</span></span> | <span data-ttu-id="c10e3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c10e3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c10e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c10e3-123">Authorization</span></span>  | <span data-ttu-id="c10e3-124">string</span><span class="sxs-lookup"><span data-stu-id="c10e3-124">string</span></span>  | <span data-ttu-id="c10e3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c10e3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c10e3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c10e3-127">Request body</span></span>
<span data-ttu-id="c10e3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c10e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c10e3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c10e3-129">Response</span></span>

<span data-ttu-id="c10e3-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c10e3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c10e3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c10e3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c10e3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c10e3-133">Request</span></span>
<span data-ttu-id="c10e3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c10e3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="c10e3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="c10e3-135">Response</span></span>
<span data-ttu-id="c10e3-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c10e3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
