---
title: Обновление принтера
description: Обновление свойств совместной работы принтера. Этот метод можно использовать для "замены" принтеров.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ebcf17c40b3d9175ec9db4c9621ebfc053647c1d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037451"
---
# <a name="update-printershare"></a><span data-ttu-id="f6c7f-104">Обновление принтера</span><span class="sxs-lookup"><span data-stu-id="f6c7f-104">Update printershare</span></span>

<span data-ttu-id="f6c7f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c7f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6c7f-106">Обновление свойств совместной работы принтера.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-106">Update the properties of a printer share.</span></span> <span data-ttu-id="f6c7f-107">Этот метод можно использовать для замены [принтеров.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="f6c7f-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="f6c7f-108">Например, если устройство физического принтера ломается, [](../resources/printer.md) администратор может [](../resources/printerShare.md) зарегистрировать новое устройство принтера и обновить этот принтер, чтобы указать на новый принтер, не требуя от пользователей каких-либо действий.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c7f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6c7f-109">Permissions</span></span>
<span data-ttu-id="f6c7f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6c7f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f6c7f-112">Помимо следующих разрешений, клиент или клиент приложения должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="f6c7f-113">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="f6c7f-113">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f6c7f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6c7f-114">Permission type</span></span> | <span data-ttu-id="f6c7f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6c7f-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f6c7f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6c7f-116">Delegated (work or school account)</span></span>| <span data-ttu-id="f6c7f-117">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c7f-117">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="f6c7f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6c7f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6c7f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-119">Not Supported.</span></span>|
|<span data-ttu-id="f6c7f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6c7f-120">Application</span></span>|<span data-ttu-id="f6c7f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6c7f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6c7f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/shares/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f6c7f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6c7f-123">Request headers</span></span>
| <span data-ttu-id="f6c7f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f6c7f-124">Name</span></span>       | <span data-ttu-id="f6c7f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f6c7f-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f6c7f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6c7f-126">Authorization</span></span> | <span data-ttu-id="f6c7f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6c7f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6c7f-129">Content-type</span></span>  | <span data-ttu-id="f6c7f-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6c7f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6c7f-132">Request body</span></span>
<span data-ttu-id="f6c7f-133">В теле запроса укажи значения для соответствующих полей [printerShare,](../resources/printershare.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-133">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="f6c7f-134">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f6c7f-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-135">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="f6c7f-136">Следующие свойства можно обновить:</span><span class="sxs-lookup"><span data-stu-id="f6c7f-136">Following properties can be updated:</span></span> 

| <span data-ttu-id="f6c7f-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6c7f-137">Property</span></span>     | <span data-ttu-id="f6c7f-138">Тип</span><span class="sxs-lookup"><span data-stu-id="f6c7f-138">Type</span></span>        | <span data-ttu-id="f6c7f-139">Описание</span><span class="sxs-lookup"><span data-stu-id="f6c7f-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f6c7f-140">принтер</span><span class="sxs-lookup"><span data-stu-id="f6c7f-140">printer</span></span>|<span data-ttu-id="f6c7f-141">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="f6c7f-141">microsoft.graph.printer</span></span>|<span data-ttu-id="f6c7f-142">Принтер, с который связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-142">The printer that this printer share is related to.</span></span> <span data-ttu-id="f6c7f-143">Используйте синтаксис, как показано в следующем примере, чтобы обновить принтер, с которым связан этот `printer@odata.bind` принтер.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-143">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|
|<span data-ttu-id="f6c7f-144">displayName</span><span class="sxs-lookup"><span data-stu-id="f6c7f-144">displayName</span></span>|<span data-ttu-id="f6c7f-145">String</span><span class="sxs-lookup"><span data-stu-id="f6c7f-145">String</span></span>|<span data-ttu-id="f6c7f-146">Имя доли принтера, которую должны отображать клиенты печати.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-146">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="f6c7f-147">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="f6c7f-147">allowAllUsers</span></span>|<span data-ttu-id="f6c7f-148">Логический</span><span class="sxs-lookup"><span data-stu-id="f6c7f-148">Boolean</span></span>| <span data-ttu-id="f6c7f-149">Если это так, всем пользователям и группам будет предоставлен доступ к этой совместной печати.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-149">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="f6c7f-150">Это замещеет списки разрешенных объектов, определенные свойствами allowedUsers и allowedGroups.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-150">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|

## <a name="response"></a><span data-ttu-id="f6c7f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6c7f-151">Response</span></span>
<span data-ttu-id="f6c7f-152">В случае успешного использования этот метод возвращает код отклика и обновленный объект `200 OK` [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-152">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6c7f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="f6c7f-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6c7f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6c7f-154">Request</span></span>
<span data-ttu-id="f6c7f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6c7f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6c7f-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/shares/{id}
Content-type: application/json
Content-length: 109

{
  "displayName": "ShareName",
  "allowAllUsers": true,
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="f6c7f-157">C#</span><span class="sxs-lookup"><span data-stu-id="f6c7f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6c7f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6c7f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6c7f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6c7f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6c7f-160">Java</span><span class="sxs-lookup"><span data-stu-id="f6c7f-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f6c7f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6c7f-161">Response</span></span>
<span data-ttu-id="f6c7f-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-162">The following is an example of the response.</span></span>
><span data-ttu-id="f6c7f-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f6c7f-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": true,
  "status": {
    "state": "stopped",
    "details": ["disconnected"],
    "description": ""
  }
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
