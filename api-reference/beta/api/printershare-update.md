---
title: Обновление принтершаре
description: Обновление свойств общего принтера. Этот метод можно использовать для "перекачки" принтеров.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9bf2e35889a99facd6e015209379e91feeec17b4
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314778"
---
# <a name="update-printershare"></a><span data-ttu-id="0e378-104">Обновление принтершаре</span><span class="sxs-lookup"><span data-stu-id="0e378-104">Update printershare</span></span>

<span data-ttu-id="0e378-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e378-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e378-106">Обновление свойств общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="0e378-106">Update the properties of a printer share.</span></span> <span data-ttu-id="0e378-107">Этот метод можно использовать для замены [принтеров](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="0e378-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="0e378-108">Например, если устройство физического принтера прерывается, администратор может зарегистрировать новое печатающее устройство и обновить эту [принтершаре](../resources/printerShare.md) , чтобы указать на [новый принтер,](../resources/printer.md) не требуя от пользователей предпринимать никаких действий.</span><span class="sxs-lookup"><span data-stu-id="0e378-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e378-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e378-109">Permissions</span></span>
<span data-ttu-id="0e378-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e378-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0e378-112">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="0e378-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="0e378-113">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="0e378-113">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0e378-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e378-114">Permission type</span></span> | <span data-ttu-id="0e378-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e378-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0e378-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e378-116">Delegated (work or school account)</span></span>| <span data-ttu-id="0e378-117">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e378-117">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="0e378-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e378-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e378-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e378-119">Not Supported.</span></span>|
|<span data-ttu-id="0e378-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e378-120">Application</span></span>|<span data-ttu-id="0e378-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e378-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e378-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e378-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/shares/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e378-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e378-123">Request headers</span></span>
| <span data-ttu-id="0e378-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0e378-124">Name</span></span>       | <span data-ttu-id="0e378-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0e378-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0e378-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e378-126">Authorization</span></span> | <span data-ttu-id="0e378-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e378-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e378-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e378-129">Content-type</span></span>  | <span data-ttu-id="0e378-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e378-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e378-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e378-132">Request body</span></span>
<span data-ttu-id="0e378-133">В тексте запроса укажите значения для соответствующих полей [принтершаре](../resources/printershare.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0e378-133">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="0e378-134">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="0e378-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0e378-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0e378-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e378-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e378-136">Property</span></span>     | <span data-ttu-id="0e378-137">Тип</span><span class="sxs-lookup"><span data-stu-id="0e378-137">Type</span></span>        | <span data-ttu-id="0e378-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0e378-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e378-139">Printer</span><span class="sxs-lookup"><span data-stu-id="0e378-139">printer</span></span>|<span data-ttu-id="0e378-140">String</span><span class="sxs-lookup"><span data-stu-id="0e378-140">String</span></span>|<span data-ttu-id="0e378-141">Принтер, с которым связан этот общий принтер.</span><span class="sxs-lookup"><span data-stu-id="0e378-141">The printer that this printer share is related to.</span></span> <span data-ttu-id="0e378-142">Используйте `printer@odata.bind` синтаксис, как показано в следующем примере, чтобы обновить принтер, с которым связан этот общий принтер.</span><span class="sxs-lookup"><span data-stu-id="0e378-142">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|

><span data-ttu-id="0e378-143">**Примечание:** Обновление имени общего принтера не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e378-143">**Note:** Updating the printer share name is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="0e378-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e378-144">Response</span></span>
<span data-ttu-id="0e378-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e378-145">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e378-146">Пример</span><span class="sxs-lookup"><span data-stu-id="0e378-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e378-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e378-147">Request</span></span>
<span data-ttu-id="0e378-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e378-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e378-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e378-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/shares/{id}
Content-type: application/json
Content-length: 109

{
  "name": "ShareName",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="0e378-150">C#</span><span class="sxs-lookup"><span data-stu-id="0e378-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e378-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e378-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e378-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e378-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0e378-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e378-153">Response</span></span>
<span data-ttu-id="0e378-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e378-154">The following is an example of the response.</span></span>
><span data-ttu-id="0e378-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e378-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "name": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printershare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->