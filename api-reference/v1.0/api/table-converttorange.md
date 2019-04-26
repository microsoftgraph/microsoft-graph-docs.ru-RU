---
title: 'Table: convertToRange'
description: Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2cda7e4eac082938cafb8328063658071eeb01d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560853"
---
# <a name="table-converttorange"></a><span data-ttu-id="547fd-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="547fd-104">Table: convertToRange</span></span>

<span data-ttu-id="547fd-p102">Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.</span><span class="sxs-lookup"><span data-stu-id="547fd-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="547fd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="547fd-107">Permissions</span></span>
<span data-ttu-id="547fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="547fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="547fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="547fd-110">Permission type</span></span>      | <span data-ttu-id="547fd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="547fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="547fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="547fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="547fd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="547fd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="547fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="547fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="547fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="547fd-115">Not supported.</span></span>    |
|<span data-ttu-id="547fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="547fd-116">Application</span></span> | <span data-ttu-id="547fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="547fd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="547fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="547fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="547fd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="547fd-119">Request headers</span></span>
| <span data-ttu-id="547fd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="547fd-120">Name</span></span>       | <span data-ttu-id="547fd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="547fd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="547fd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="547fd-122">Authorization</span></span>  | <span data-ttu-id="547fd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="547fd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="547fd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="547fd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="547fd-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="547fd-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="547fd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="547fd-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="547fd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="547fd-129">Response</span></span>

<span data-ttu-id="547fd-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="547fd-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="547fd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="547fd-131">Example</span></span>
<span data-ttu-id="547fd-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="547fd-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="547fd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="547fd-133">Request</span></span>
<span data-ttu-id="547fd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="547fd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="547fd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="547fd-135">Response</span></span>
<span data-ttu-id="547fd-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="547fd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
