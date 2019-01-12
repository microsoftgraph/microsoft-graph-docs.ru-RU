---
title: Создание объекта ChartPoints
description: С помощью этого API можно создать объект ChartPoints.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3c7ee1257dbe32169b6619b6c2d185bf37d39b7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921453"
---
# <a name="create-chartpoints"></a><span data-ttu-id="c3d36-103">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="c3d36-103">Create ChartPoints</span></span>

> <span data-ttu-id="c3d36-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3d36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3d36-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3d36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3d36-106">С помощью этого API можно создать объект ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="c3d36-106">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3d36-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3d36-107">Permissions</span></span>
<span data-ttu-id="c3d36-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3d36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3d36-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3d36-110">Permission type</span></span>      | <span data-ttu-id="c3d36-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3d36-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3d36-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3d36-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c3d36-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3d36-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c3d36-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3d36-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3d36-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3d36-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c3d36-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3d36-116">Application</span></span> | <span data-ttu-id="c3d36-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3d36-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3d36-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3d36-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="c3d36-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3d36-119">Request headers</span></span>
| <span data-ttu-id="c3d36-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c3d36-120">Name</span></span>       | <span data-ttu-id="c3d36-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c3d36-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c3d36-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3d36-122">Authorization</span></span>  | <span data-ttu-id="c3d36-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3d36-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3d36-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c3d36-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c3d36-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c3d36-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3d36-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3d36-128">Request body</span></span>
<span data-ttu-id="c3d36-129">Предоставьте в тексте запроса описание объекта [ChartPoints](../resources/chartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3d36-129">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c3d36-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d36-130">Response</span></span>

<span data-ttu-id="c3d36-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ChartPoints](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3d36-131">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3d36-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c3d36-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3d36-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3d36-133">Request</span></span>
<span data-ttu-id="c3d36-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3d36-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="c3d36-135">Предоставьте в тексте запроса описание объекта [ChartPoints](../resources/chartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3d36-135">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c3d36-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d36-136">Response</span></span>
<span data-ttu-id="c3d36-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c3d36-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
