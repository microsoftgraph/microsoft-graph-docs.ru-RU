---
title: Обновление принтера
description: Обновление свойств совместной работы принтера. Этот метод можно использовать для "замены" принтеров.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 991364b3d1900fc99c41cfb55a2e26cff505167d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776825"
---
# <a name="update-printershare"></a><span data-ttu-id="ca912-104">Обновление printerShare</span><span class="sxs-lookup"><span data-stu-id="ca912-104">Update printerShare</span></span>
<span data-ttu-id="ca912-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca912-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="ca912-106">Обновление свойств совместной работы принтера.</span><span class="sxs-lookup"><span data-stu-id="ca912-106">Update the properties of a printer share.</span></span> <span data-ttu-id="ca912-107">Этот метод можно использовать для замены [принтеров.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="ca912-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="ca912-108">Например, если устройство физического принтера ломается, [](../resources/printer.md) администратор может [](../resources/printerShare.md) зарегистрировать новое устройство принтера и обновить этот принтер, чтобы указать на новый принтер, не требуя от пользователей каких-либо действий.</span><span class="sxs-lookup"><span data-stu-id="ca912-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca912-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca912-109">Permissions</span></span>
<span data-ttu-id="ca912-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca912-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ca912-112">Помимо следующих разрешений, клиент или клиент приложения должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="ca912-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="ca912-113">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="ca912-113">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ca912-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca912-114">Permission type</span></span> | <span data-ttu-id="ca912-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca912-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ca912-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca912-116">Delegated (work or school account)</span></span>| <span data-ttu-id="ca912-117">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca912-117">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="ca912-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca912-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca912-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca912-119">Not Supported.</span></span>|
|<span data-ttu-id="ca912-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca912-120">Application</span></span>|<span data-ttu-id="ca912-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca912-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca912-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca912-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/shares/{printerShareId}
```

## <a name="request-headers"></a><span data-ttu-id="ca912-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca912-123">Request headers</span></span>
|<span data-ttu-id="ca912-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ca912-124">Name</span></span>|<span data-ttu-id="ca912-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ca912-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ca912-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca912-126">Authorization</span></span>|<span data-ttu-id="ca912-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca912-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ca912-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca912-129">Content-Type</span></span>|<span data-ttu-id="ca912-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca912-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca912-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca912-132">Request body</span></span>
<span data-ttu-id="ca912-133">В теле запроса укажи значения для соответствующих полей [printerShare,](../resources/printershare.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="ca912-133">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="ca912-134">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="ca912-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ca912-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ca912-135">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="ca912-136">Следующие свойства можно обновить:</span><span class="sxs-lookup"><span data-stu-id="ca912-136">Following properties can be updated:</span></span> 

| <span data-ttu-id="ca912-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca912-137">Property</span></span>     | <span data-ttu-id="ca912-138">Тип</span><span class="sxs-lookup"><span data-stu-id="ca912-138">Type</span></span>        | <span data-ttu-id="ca912-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ca912-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca912-140">printer</span><span class="sxs-lookup"><span data-stu-id="ca912-140">printer</span></span>|<span data-ttu-id="ca912-141">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="ca912-141">microsoft.graph.printer</span></span>|<span data-ttu-id="ca912-142">Принтер, с который связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="ca912-142">The printer that this printer share is related to.</span></span> <span data-ttu-id="ca912-143">Используйте синтаксис, как показано в следующем примере, чтобы обновить принтер, с которым связан этот `printer@odata.bind` принтер.</span><span class="sxs-lookup"><span data-stu-id="ca912-143">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|
|<span data-ttu-id="ca912-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ca912-144">displayName</span></span>|<span data-ttu-id="ca912-145">String</span><span class="sxs-lookup"><span data-stu-id="ca912-145">String</span></span>|<span data-ttu-id="ca912-146">Имя доли принтера, которую должны отображать клиенты печати.</span><span class="sxs-lookup"><span data-stu-id="ca912-146">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="ca912-147">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="ca912-147">allowAllUsers</span></span>|<span data-ttu-id="ca912-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca912-148">Boolean</span></span>| <span data-ttu-id="ca912-149">Если это так, всем пользователям и группам будет предоставлен доступ к этой совместной печати.</span><span class="sxs-lookup"><span data-stu-id="ca912-149">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="ca912-150">Это замещеет списки разрешенных объектов, определенные свойствами allowedUsers и allowedGroups.</span><span class="sxs-lookup"><span data-stu-id="ca912-150">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|

## <a name="response"></a><span data-ttu-id="ca912-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca912-151">Response</span></span>

<span data-ttu-id="ca912-152">В случае успешного использования этот метод возвращает код отклика и обновленный объект `200 OK` [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca912-152">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca912-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca912-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca912-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca912-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ca912-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca912-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
Content-Type: application/json
Content-length: 509

{
  "displayName": "PrinterShare Name",
  "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}",
  "allowAllUsers": false
}
```
# <a name="c"></a>[<span data-ttu-id="ca912-156">C#</span><span class="sxs-lookup"><span data-stu-id="ca912-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca912-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca912-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca912-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca912-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca912-159">Java</span><span class="sxs-lookup"><span data-stu-id="ca912-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca912-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca912-160">Response</span></span>
<span data-ttu-id="ca912-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca912-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "PrinterShare Name",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "status": {
    "state": "stopped",
    "details": ["disconnected"],
    "description": ""
  }
}
```

