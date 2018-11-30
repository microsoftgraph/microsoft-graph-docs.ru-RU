---
title: Обновление объекта ChartTitle
description: Обновление свойств объекта charttitle.
ms.openlocfilehash: a20cafee793c5622fe29ad57aafb8e3d1e5cd2b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075679"
---
# <a name="update-charttitle"></a><span data-ttu-id="71b7e-103">Обновление объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="71b7e-103">Update charttitle</span></span>

> <span data-ttu-id="71b7e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71b7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71b7e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b7e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71b7e-106">Обновление свойств объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="71b7e-106">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="71b7e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71b7e-107">Permissions</span></span>
<span data-ttu-id="71b7e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71b7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71b7e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71b7e-110">Permission type</span></span>      | <span data-ttu-id="71b7e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71b7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71b7e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71b7e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71b7e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71b7e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71b7e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71b7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b7e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71b7e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71b7e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71b7e-116">Application</span></span> | <span data-ttu-id="71b7e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b7e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71b7e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71b7e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="71b7e-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71b7e-119">Optional request headers</span></span>
| <span data-ttu-id="71b7e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="71b7e-120">Name</span></span>       | <span data-ttu-id="71b7e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71b7e-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="71b7e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71b7e-122">Authorization</span></span>  | <span data-ttu-id="71b7e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71b7e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71b7e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71b7e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="71b7e-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="71b7e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71b7e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71b7e-128">Request body</span></span>
<span data-ttu-id="71b7e-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="71b7e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="71b7e-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="71b7e-132">Property</span></span>     | <span data-ttu-id="71b7e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="71b7e-133">Type</span></span>   |<span data-ttu-id="71b7e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="71b7e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71b7e-135">overlay</span><span class="sxs-lookup"><span data-stu-id="71b7e-135">overlay</span></span>|<span data-ttu-id="71b7e-136">boolean</span><span class="sxs-lookup"><span data-stu-id="71b7e-136">boolean</span></span>|<span data-ttu-id="71b7e-137">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="71b7e-137">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="71b7e-138">text</span><span class="sxs-lookup"><span data-stu-id="71b7e-138">text</span></span>|<span data-ttu-id="71b7e-139">строка</span><span class="sxs-lookup"><span data-stu-id="71b7e-139">string</span></span>|<span data-ttu-id="71b7e-140">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="71b7e-140">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="71b7e-141">visible</span><span class="sxs-lookup"><span data-stu-id="71b7e-141">visible</span></span>|<span data-ttu-id="71b7e-142">boolean</span><span class="sxs-lookup"><span data-stu-id="71b7e-142">boolean</span></span>|<span data-ttu-id="71b7e-143">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="71b7e-143">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="71b7e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b7e-144">Response</span></span>

<span data-ttu-id="71b7e-145">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartTitle](../resources/charttitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71b7e-145">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71b7e-146">Пример</span><span class="sxs-lookup"><span data-stu-id="71b7e-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71b7e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="71b7e-147">Request</span></span>
<span data-ttu-id="71b7e-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71b7e-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="71b7e-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="71b7e-149">Response</span></span>
<span data-ttu-id="71b7e-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="71b7e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->