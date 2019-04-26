---
title: 'workbookRangeView: range'
description: Возвращение диапазона, связанного с ресурсом rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d4a97773f255e08e54be0360fc443f1193884fae
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339619"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="51aa4-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="51aa4-103">workbookRangeView: range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51aa4-104">Возвращение диапазона, связанного с ресурсом rangeView.</span><span class="sxs-lookup"><span data-stu-id="51aa4-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="51aa4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51aa4-105">Permissions</span></span>
<span data-ttu-id="51aa4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="51aa4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51aa4-108">Permission type</span></span>      | <span data-ttu-id="51aa4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51aa4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51aa4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51aa4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="51aa4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51aa4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="51aa4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51aa4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51aa4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51aa4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="51aa4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51aa4-114">Application</span></span> | <span data-ttu-id="51aa4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51aa4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51aa4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51aa4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="51aa4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51aa4-117">Request headers</span></span>
| <span data-ttu-id="51aa4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="51aa4-118">Name</span></span>       | <span data-ttu-id="51aa4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="51aa4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="51aa4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51aa4-120">Authorization</span></span>  | <span data-ttu-id="51aa4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51aa4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51aa4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="51aa4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="51aa4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="51aa4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51aa4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51aa4-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="51aa4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="51aa4-127">Response</span></span>

<span data-ttu-id="51aa4-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51aa4-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51aa4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="51aa4-129">Example</span></span>
<span data-ttu-id="51aa4-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="51aa4-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51aa4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="51aa4-131">Request</span></span>
<span data-ttu-id="51aa4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51aa4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="51aa4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="51aa4-133">Response</span></span>
<span data-ttu-id="51aa4-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51aa4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
