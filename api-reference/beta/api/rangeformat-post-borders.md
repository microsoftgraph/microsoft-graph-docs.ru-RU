---
title: Создание объекта RangeBorder
description: С помощью этого API можно создать объект RangeBorder.
author: lumine2008
ms.openlocfilehash: d5908c149b91aa81e30482fdc995cca0126ada2b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337417"
---
# <a name="create-rangeborder"></a><span data-ttu-id="56e1b-103">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="56e1b-103">Create RangeBorder</span></span>

> <span data-ttu-id="56e1b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56e1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56e1b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56e1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56e1b-106">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="56e1b-106">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="56e1b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56e1b-107">Permissions</span></span>
<span data-ttu-id="56e1b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56e1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56e1b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56e1b-110">Permission type</span></span>      | <span data-ttu-id="56e1b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56e1b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56e1b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56e1b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="56e1b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56e1b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56e1b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56e1b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56e1b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56e1b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56e1b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56e1b-116">Application</span></span> | <span data-ttu-id="56e1b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56e1b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56e1b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56e1b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="56e1b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56e1b-119">Request headers</span></span>
| <span data-ttu-id="56e1b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="56e1b-120">Name</span></span>       | <span data-ttu-id="56e1b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="56e1b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56e1b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56e1b-122">Authorization</span></span>  | <span data-ttu-id="56e1b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56e1b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56e1b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="56e1b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="56e1b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="56e1b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56e1b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56e1b-128">Request body</span></span>
<span data-ttu-id="56e1b-129">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56e1b-129">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="56e1b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="56e1b-130">Response</span></span>

<span data-ttu-id="56e1b-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56e1b-131">If successful, this method returns `201 Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56e1b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="56e1b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56e1b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="56e1b-133">Request</span></span>
<span data-ttu-id="56e1b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56e1b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="56e1b-135">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56e1b-135">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="56e1b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="56e1b-136">Response</span></span>
<span data-ttu-id="56e1b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="56e1b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->