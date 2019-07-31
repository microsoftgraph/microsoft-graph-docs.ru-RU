---
title: 'workbookRange: visibleView'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f91b5044c470430d8d508cab3585db48b51048bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995869"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="c8497-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="c8497-104">workbookRange: visibleView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="c8497-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8497-105">Permissions</span></span>
<span data-ttu-id="c8497-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8497-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8497-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8497-108">Permission type</span></span>      | <span data-ttu-id="c8497-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8497-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8497-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8497-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8497-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8497-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8497-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8497-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8497-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8497-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8497-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8497-114">Application</span></span> | <span data-ttu-id="c8497-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8497-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8497-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8497-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="c8497-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8497-117">Request headers</span></span>
| <span data-ttu-id="c8497-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c8497-118">Name</span></span>       | <span data-ttu-id="c8497-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c8497-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8497-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8497-120">Authorization</span></span>  | <span data-ttu-id="c8497-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8497-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8497-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c8497-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8497-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c8497-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8497-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8497-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c8497-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8497-127">Response</span></span>

<span data-ttu-id="c8497-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c8497-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8497-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c8497-129">Example</span></span>
<span data-ttu-id="c8497-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c8497-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8497-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8497-131">Request</span></span>
<span data-ttu-id="c8497-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8497-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="c8497-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8497-133">Response</span></span>
<span data-ttu-id="c8497-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8497-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
