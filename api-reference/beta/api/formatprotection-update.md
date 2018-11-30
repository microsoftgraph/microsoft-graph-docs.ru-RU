---
title: Обновление объекта FormatProtection
description: Обновление свойств объекта FormatProtection.
ms.openlocfilehash: 7a75af3b340b194df16a53dd7800d5d6981730ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078297"
---
# <a name="update-formatprotection"></a><span data-ttu-id="4b571-103">Обновление объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="4b571-103">Update formatprotection</span></span>

> <span data-ttu-id="4b571-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b571-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b571-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b571-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b571-106">Обновление свойств объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="4b571-106">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b571-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b571-107">Permissions</span></span>
<span data-ttu-id="4b571-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b571-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b571-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b571-110">Permission type</span></span>      | <span data-ttu-id="4b571-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b571-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b571-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b571-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4b571-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b571-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b571-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b571-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b571-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b571-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b571-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b571-116">Application</span></span> | <span data-ttu-id="4b571-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b571-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b571-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b571-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="4b571-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b571-119">Optional request headers</span></span>
| <span data-ttu-id="4b571-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4b571-120">Name</span></span>       | <span data-ttu-id="4b571-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4b571-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4b571-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b571-122">Authorization</span></span>  | <span data-ttu-id="4b571-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b571-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b571-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b571-125">Request body</span></span>
<span data-ttu-id="4b571-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4b571-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b571-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b571-129">Property</span></span>     | <span data-ttu-id="4b571-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b571-130">Type</span></span>   |<span data-ttu-id="4b571-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b571-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b571-132">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="4b571-132">formulaHidden</span></span>|<span data-ttu-id="4b571-133">boolean</span><span class="sxs-lookup"><span data-stu-id="4b571-133">boolean</span></span>|<span data-ttu-id="4b571-p105">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="4b571-p105">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="4b571-136">locked</span><span class="sxs-lookup"><span data-stu-id="4b571-136">locked</span></span>|<span data-ttu-id="4b571-137">boolean</span><span class="sxs-lookup"><span data-stu-id="4b571-137">boolean</span></span>|<span data-ttu-id="4b571-p106">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="4b571-p106">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="4b571-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b571-140">Response</span></span>

<span data-ttu-id="4b571-141">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [FormatProtection](../resources/formatprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b571-141">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b571-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4b571-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b571-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b571-143">Request</span></span>
<span data-ttu-id="4b571-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b571-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="4b571-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b571-145">Response</span></span>
<span data-ttu-id="4b571-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4b571-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->