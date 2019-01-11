---
title: 'workbookRange: visibleView'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
ms.openlocfilehash: f994866c8f55ec2ffbc0b680d4576fbc6a8b7bb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875168"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="4f579-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="4f579-104">workbookRange: visibleView</span></span>

> <span data-ttu-id="4f579-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f579-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f579-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f579-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f579-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f579-107">Permissions</span></span>
<span data-ttu-id="4f579-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f579-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f579-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f579-110">Permission type</span></span>      | <span data-ttu-id="4f579-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f579-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f579-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f579-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4f579-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f579-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f579-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f579-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f579-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f579-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f579-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f579-116">Application</span></span> | <span data-ttu-id="4f579-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f579-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f579-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f579-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="4f579-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f579-119">Request headers</span></span>
| <span data-ttu-id="4f579-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4f579-120">Name</span></span>       | <span data-ttu-id="4f579-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4f579-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f579-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f579-122">Authorization</span></span>  | <span data-ttu-id="4f579-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f579-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f579-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4f579-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f579-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4f579-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f579-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f579-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4f579-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f579-129">Response</span></span>

<span data-ttu-id="4f579-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f579-130">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f579-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4f579-131">Example</span></span>
<span data-ttu-id="4f579-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4f579-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4f579-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f579-133">Request</span></span>
<span data-ttu-id="4f579-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f579-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="4f579-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f579-135">Response</span></span>
<span data-ttu-id="4f579-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4f579-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
