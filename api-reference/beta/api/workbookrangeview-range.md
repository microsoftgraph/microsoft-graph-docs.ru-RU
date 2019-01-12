---
title: 'workbookRangeView: range'
description: Возвращение диапазона, связанного с ресурсом rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 616d65c490f7691ec8ab83ffd12eaba480f4734a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970908"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="01612-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="01612-103">workbookRangeView: range</span></span>

> <span data-ttu-id="01612-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01612-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01612-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01612-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01612-106">Возвращение диапазона, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="01612-106">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="01612-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01612-107">Permissions</span></span>
<span data-ttu-id="01612-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01612-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="01612-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01612-110">Permission type</span></span>      | <span data-ttu-id="01612-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01612-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01612-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01612-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01612-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01612-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01612-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01612-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01612-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01612-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01612-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01612-116">Application</span></span> | <span data-ttu-id="01612-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01612-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01612-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01612-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="01612-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01612-119">Request headers</span></span>
| <span data-ttu-id="01612-120">Имя</span><span class="sxs-lookup"><span data-stu-id="01612-120">Name</span></span>       | <span data-ttu-id="01612-121">Описание</span><span class="sxs-lookup"><span data-stu-id="01612-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01612-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01612-122">Authorization</span></span>  | <span data-ttu-id="01612-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01612-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01612-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01612-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="01612-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="01612-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01612-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01612-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="01612-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="01612-129">Response</span></span>

<span data-ttu-id="01612-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01612-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01612-131">Пример</span><span class="sxs-lookup"><span data-stu-id="01612-131">Example</span></span>
<span data-ttu-id="01612-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="01612-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01612-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="01612-133">Request</span></span>
<span data-ttu-id="01612-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01612-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="01612-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="01612-135">Response</span></span>
<span data-ttu-id="01612-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="01612-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
