---
title: Создание printerShare
description: Создает новую долю принтера для указанного принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f477ce6c4a45b86677c38d2bc5d438474da46ad5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777182"
---
# <a name="create-printershare"></a><span data-ttu-id="c7827-103">Создание printerShare</span><span class="sxs-lookup"><span data-stu-id="c7827-103">Create printerShare</span></span>
<span data-ttu-id="c7827-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7827-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c7827-105">Создание нового **принтераShare** для указанного [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="c7827-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7827-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7827-106">Permissions</span></span>
<span data-ttu-id="c7827-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c7827-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c7827-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c7827-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c7827-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c7827-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7827-111">Permission type</span></span> | <span data-ttu-id="c7827-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7827-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c7827-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7827-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c7827-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7827-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="c7827-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7827-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7827-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7827-116">Not Supported.</span></span>|
|<span data-ttu-id="c7827-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7827-117">Application</span></span>|<span data-ttu-id="c7827-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7827-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7827-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7827-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares
```

## <a name="request-headers"></a><span data-ttu-id="c7827-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7827-120">Request headers</span></span>
|<span data-ttu-id="c7827-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c7827-121">Name</span></span>|<span data-ttu-id="c7827-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c7827-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7827-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7827-123">Authorization</span></span>|<span data-ttu-id="c7827-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7827-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7827-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7827-126">Content-Type</span></span>|<span data-ttu-id="c7827-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7827-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7827-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7827-129">Request body</span></span>
<span data-ttu-id="c7827-130">В теле запроса поставляем JSON-представление объекта [printerShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c7827-130">In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="c7827-131">В следующей таблице показаны свойства, которые можно предоставлять при создании [принтераShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c7827-131">The following table shows the properties that can be provided when you create the [printerShare](../resources/printershare.md).</span></span>

|<span data-ttu-id="c7827-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7827-132">Property</span></span>|<span data-ttu-id="c7827-133">Тип</span><span class="sxs-lookup"><span data-stu-id="c7827-133">Type</span></span>|<span data-ttu-id="c7827-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c7827-134">Description</span></span>|<span data-ttu-id="c7827-135">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="c7827-135">Required?</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="c7827-136">printer</span><span class="sxs-lookup"><span data-stu-id="c7827-136">printer</span></span>|<span data-ttu-id="c7827-137">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="c7827-137">microsoft.graph.printer</span></span>|<span data-ttu-id="c7827-138">Принтер, с который связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="c7827-138">The printer that this printer share is related to.</span></span> <span data-ttu-id="c7827-139">Используйте `printer@odata.bind` синтаксис, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="c7827-139">Use the `printer@odata.bind` syntax, as shown in the following example.</span></span>|<span data-ttu-id="c7827-140">Да</span><span class="sxs-lookup"><span data-stu-id="c7827-140">Yes</span></span>|
|<span data-ttu-id="c7827-141">displayName</span><span class="sxs-lookup"><span data-stu-id="c7827-141">displayName</span></span>|<span data-ttu-id="c7827-142">String</span><span class="sxs-lookup"><span data-stu-id="c7827-142">String</span></span>|<span data-ttu-id="c7827-143">Имя доли принтера, которую должны отображать клиенты печати.</span><span class="sxs-lookup"><span data-stu-id="c7827-143">The name of the printer share that print clients should display.</span></span> <span data-ttu-id="c7827-144">Максимальная разрешенная длина — 50 символов.</span><span class="sxs-lookup"><span data-stu-id="c7827-144">Maximum length allowed is 50 characters.</span></span>|<span data-ttu-id="c7827-145">Да</span><span class="sxs-lookup"><span data-stu-id="c7827-145">Yes</span></span>|
|<span data-ttu-id="c7827-146">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="c7827-146">allowAllUsers</span></span>|<span data-ttu-id="c7827-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7827-147">Boolean</span></span>|<span data-ttu-id="c7827-148">Если всем пользователям и группам будет предоставлен доступ `true` к этой совместной печати.</span><span class="sxs-lookup"><span data-stu-id="c7827-148">If `true`, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="c7827-149">Это замещеет списки разрешенных объектов, определенные **свойствами allowedUsers** и **allowedGroups.**</span><span class="sxs-lookup"><span data-stu-id="c7827-149">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|<span data-ttu-id="c7827-150">Нет</span><span class="sxs-lookup"><span data-stu-id="c7827-150">No</span></span>|

## <a name="response"></a><span data-ttu-id="c7827-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7827-151">Response</span></span>

<span data-ttu-id="c7827-152">В случае успешного использования этот метод возвращает код отклика и `201 Created` объект [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7827-152">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7827-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7827-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7827-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7827-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7827-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7827-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares
Content-Type: application/json
Content-length: 509

{
  "displayName": "ShareName",
  "allowAllUsers": false,
  "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}"
}
```
# <a name="c"></a>[<span data-ttu-id="c7827-156">C#</span><span class="sxs-lookup"><span data-stu-id="c7827-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printershare-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7827-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7827-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printershare-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7827-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7827-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printershare-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7827-159">Java</span><span class="sxs-lookup"><span data-stu-id="c7827-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printershare-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7827-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7827-160">Response</span></span>
<span data-ttu-id="c7827-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7827-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "status": {
    "state": "ready",
    "details": [],
    "description": ""
  }
}
```

