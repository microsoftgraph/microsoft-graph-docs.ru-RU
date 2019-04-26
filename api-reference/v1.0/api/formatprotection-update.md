---
title: Обновление объекта FormatProtection
description: Обновление свойств объекта FormatProtection.
localization_priority: Normal
ms.openlocfilehash: 26e51babc4610c331563923c464db341d4517c51
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563845"
---
# <a name="update-formatprotection"></a><span data-ttu-id="1d277-103">Обновление объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="1d277-103">Update formatprotection</span></span>

<span data-ttu-id="1d277-104">Обновление свойств объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="1d277-104">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d277-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d277-105">Permissions</span></span>
<span data-ttu-id="1d277-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d277-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d277-108">Permission type</span></span>      | <span data-ttu-id="1d277-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d277-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="1d277-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d277-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d277-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d277-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="1d277-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d277-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d277-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d277-113">Not supported.</span></span>    | 
|<span data-ttu-id="1d277-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d277-114">Application</span></span> | <span data-ttu-id="1d277-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d277-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1d277-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d277-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="1d277-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d277-117">Optional request headers</span></span>
| <span data-ttu-id="1d277-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1d277-118">Name</span></span>       | <span data-ttu-id="1d277-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1d277-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1d277-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d277-120">Authorization</span></span>  | <span data-ttu-id="1d277-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d277-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1d277-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d277-123">Request body</span></span>
<span data-ttu-id="1d277-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1d277-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d277-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d277-127">Property</span></span>     | <span data-ttu-id="1d277-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1d277-128">Type</span></span>   |<span data-ttu-id="1d277-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1d277-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d277-130">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="1d277-130">formulaHidden</span></span>|<span data-ttu-id="1d277-131">boolean</span><span class="sxs-lookup"><span data-stu-id="1d277-131">boolean</span></span>|<span data-ttu-id="1d277-p104">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="1d277-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="1d277-134">locked</span><span class="sxs-lookup"><span data-stu-id="1d277-134">locked</span></span>|<span data-ttu-id="1d277-135">boolean</span><span class="sxs-lookup"><span data-stu-id="1d277-135">boolean</span></span>|<span data-ttu-id="1d277-p105">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="1d277-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="1d277-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d277-138">Response</span></span>

<span data-ttu-id="1d277-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [FormatProtection](../resources/formatprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d277-139">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d277-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1d277-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d277-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d277-141">Request</span></span>
<span data-ttu-id="1d277-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d277-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="1d277-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d277-143">Response</span></span>
<span data-ttu-id="1d277-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d277-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
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
