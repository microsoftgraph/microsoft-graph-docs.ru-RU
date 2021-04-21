---
title: Создание printerShare
description: Создает новую долю принтера для указанного принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6c721c4c7b4e534fc22e71db221c73670b5e477a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921151"
---
# <a name="create-printershare"></a><span data-ttu-id="27dcb-103">Создание printerShare</span><span class="sxs-lookup"><span data-stu-id="27dcb-103">Create printerShare</span></span>

<span data-ttu-id="27dcb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27dcb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27dcb-105">Создание нового **принтераShare** для указанного [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="27dcb-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="27dcb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27dcb-106">Permissions</span></span>
<span data-ttu-id="27dcb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27dcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="27dcb-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="27dcb-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="27dcb-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="27dcb-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="27dcb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27dcb-111">Permission type</span></span> | <span data-ttu-id="27dcb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27dcb-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="27dcb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27dcb-113">Delegated (work or school account)</span></span>| <span data-ttu-id="27dcb-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27dcb-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="27dcb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27dcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27dcb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27dcb-116">Not Supported.</span></span>|
|<span data-ttu-id="27dcb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="27dcb-117">Application</span></span>|<span data-ttu-id="27dcb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27dcb-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27dcb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27dcb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares
```
## <a name="request-headers"></a><span data-ttu-id="27dcb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27dcb-120">Request headers</span></span>
| <span data-ttu-id="27dcb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="27dcb-121">Name</span></span>          | <span data-ttu-id="27dcb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="27dcb-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27dcb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27dcb-123">Authorization</span></span> | <span data-ttu-id="27dcb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27dcb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27dcb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27dcb-126">Content-type</span></span>  | <span data-ttu-id="27dcb-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27dcb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27dcb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27dcb-129">Request body</span></span>
<span data-ttu-id="27dcb-130">В теле запроса поставляем JSON-представление объекта [printerShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="27dcb-130">In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="27dcb-131">В следующей таблице показаны свойства, которые можно предоставлять при создании [принтераShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="27dcb-131">The following table shows the properties that can be provided when you create the [printerShare](../resources/printershare.md).</span></span>

|<span data-ttu-id="27dcb-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="27dcb-132">Property</span></span>|<span data-ttu-id="27dcb-133">Тип</span><span class="sxs-lookup"><span data-stu-id="27dcb-133">Type</span></span>|<span data-ttu-id="27dcb-134">Описание</span><span class="sxs-lookup"><span data-stu-id="27dcb-134">Description</span></span>|<span data-ttu-id="27dcb-135">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="27dcb-135">Required?</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="27dcb-136">принтер</span><span class="sxs-lookup"><span data-stu-id="27dcb-136">printer</span></span>|<span data-ttu-id="27dcb-137">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="27dcb-137">microsoft.graph.printer</span></span>|<span data-ttu-id="27dcb-138">Принтер, с который связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="27dcb-138">The printer that this printer share is related to.</span></span> <span data-ttu-id="27dcb-139">Используйте `printer@odata.bind` синтаксис, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="27dcb-139">Use the `printer@odata.bind` syntax as shown in the following example.</span></span>|<span data-ttu-id="27dcb-140">Да</span><span class="sxs-lookup"><span data-stu-id="27dcb-140">Yes</span></span>|
|<span data-ttu-id="27dcb-141">displayName</span><span class="sxs-lookup"><span data-stu-id="27dcb-141">displayName</span></span>|<span data-ttu-id="27dcb-142">Строка</span><span class="sxs-lookup"><span data-stu-id="27dcb-142">String</span></span>|<span data-ttu-id="27dcb-143">Имя доли принтера, которую должны отображать клиенты печати.</span><span class="sxs-lookup"><span data-stu-id="27dcb-143">The name of the printer share that print clients should display.</span></span> <span data-ttu-id="27dcb-144">Максимальная разрешенная длина — 50 символов.</span><span class="sxs-lookup"><span data-stu-id="27dcb-144">Maximum length allowed is 50 characters.</span></span>|<span data-ttu-id="27dcb-145">Да</span><span class="sxs-lookup"><span data-stu-id="27dcb-145">Yes</span></span>|
|<span data-ttu-id="27dcb-146">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="27dcb-146">allowAllUsers</span></span>|<span data-ttu-id="27dcb-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="27dcb-147">Boolean</span></span>| <span data-ttu-id="27dcb-148">Если это так, всем пользователям и группам будет предоставлен доступ к этой совместной печати.</span><span class="sxs-lookup"><span data-stu-id="27dcb-148">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="27dcb-149">Это замещеет списки разрешенных объектов, определенные свойствами allowedUsers и allowedGroups.</span><span class="sxs-lookup"><span data-stu-id="27dcb-149">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|<span data-ttu-id="27dcb-150">Нет</span><span class="sxs-lookup"><span data-stu-id="27dcb-150">No</span></span>|

## <a name="response"></a><span data-ttu-id="27dcb-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="27dcb-151">Response</span></span>
<span data-ttu-id="27dcb-152">В случае успешного использования этот метод возвращает код отклика и `201 Created` объект [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27dcb-152">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27dcb-153">Пример</span><span class="sxs-lookup"><span data-stu-id="27dcb-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27dcb-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="27dcb-154">Request</span></span>
<span data-ttu-id="27dcb-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27dcb-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27dcb-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="27dcb-156">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="27dcb-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="27dcb-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_print"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares
Content-type: application/json
Content-length: 114

{
  "name": "name-value",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="27dcb-158">C#</span><span class="sxs-lookup"><span data-stu-id="27dcb-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printershare-from-print-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27dcb-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27dcb-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printershare-from-print-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27dcb-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27dcb-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printershare-from-print-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27dcb-161">Java</span><span class="sxs-lookup"><span data-stu-id="27dcb-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printershare-from-print-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="27dcb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="27dcb-162">Response</span></span>
<span data-ttu-id="27dcb-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27dcb-163">The following is an example of the response.</span></span>
><span data-ttu-id="27dcb-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27dcb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 233

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
    "id": "7361c7c1-ff07-4565-9897-bef6895a7d04",
    "displayName": "ShareName",
    "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
