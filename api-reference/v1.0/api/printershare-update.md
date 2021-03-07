---
title: Обновление принтера
description: Обновление свойств совместной работы принтера. Этот метод можно использовать для "замены" принтеров.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ea7da18300105e5c177b126635740fcee918b996
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518096"
---
# <a name="update-printershare"></a><span data-ttu-id="4be8a-104">Обновление printerShare</span><span class="sxs-lookup"><span data-stu-id="4be8a-104">Update printerShare</span></span>
<span data-ttu-id="4be8a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4be8a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4be8a-106">Обновление свойств совместной работы принтера.</span><span class="sxs-lookup"><span data-stu-id="4be8a-106">Update the properties of a printer share.</span></span> <span data-ttu-id="4be8a-107">Этот метод можно использовать для замены [принтеров.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="4be8a-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="4be8a-108">Например, если устройство физического принтера ломается, [](../resources/printer.md) администратор может [](../resources/printerShare.md) зарегистрировать новое устройство принтера и обновить этот принтер, чтобы указать на новый принтер, не требуя от пользователей каких-либо действий.</span><span class="sxs-lookup"><span data-stu-id="4be8a-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="4be8a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4be8a-109">Permissions</span></span>
<span data-ttu-id="4be8a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4be8a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4be8a-112">Помимо следующих разрешений, клиент или клиент приложения должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="4be8a-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="4be8a-113">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="4be8a-113">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="4be8a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4be8a-114">Permission type</span></span> | <span data-ttu-id="4be8a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4be8a-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4be8a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4be8a-116">Delegated (work or school account)</span></span>| <span data-ttu-id="4be8a-117">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be8a-117">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="4be8a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4be8a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4be8a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4be8a-119">Not Supported.</span></span>|
|<span data-ttu-id="4be8a-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="4be8a-120">Application</span></span>|<span data-ttu-id="4be8a-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4be8a-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4be8a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4be8a-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/shares/{printerShareId}
```

## <a name="request-headers"></a><span data-ttu-id="4be8a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4be8a-123">Request headers</span></span>
|<span data-ttu-id="4be8a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4be8a-124">Name</span></span>|<span data-ttu-id="4be8a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4be8a-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4be8a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4be8a-126">Authorization</span></span>|<span data-ttu-id="4be8a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4be8a-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4be8a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4be8a-129">Content-Type</span></span>|<span data-ttu-id="4be8a-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4be8a-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4be8a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4be8a-132">Request body</span></span>
<span data-ttu-id="4be8a-133">В теле запроса укажи значения для соответствующих полей [printerShare,](../resources/printershare.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="4be8a-133">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="4be8a-134">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="4be8a-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4be8a-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4be8a-135">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="4be8a-136">Следующие свойства можно обновить:</span><span class="sxs-lookup"><span data-stu-id="4be8a-136">Following properties can be updated:</span></span> 

| <span data-ttu-id="4be8a-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="4be8a-137">Property</span></span>     | <span data-ttu-id="4be8a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="4be8a-138">Type</span></span>        | <span data-ttu-id="4be8a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="4be8a-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4be8a-140">printer</span><span class="sxs-lookup"><span data-stu-id="4be8a-140">printer</span></span>|<span data-ttu-id="4be8a-141">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="4be8a-141">microsoft.graph.printer</span></span>|<span data-ttu-id="4be8a-142">Принтер, с который связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="4be8a-142">The printer that this printer share is related to.</span></span> <span data-ttu-id="4be8a-143">Используйте синтаксис, как показано в следующем примере, чтобы обновить принтер, с которым связан этот `printer@odata.bind` принтер.</span><span class="sxs-lookup"><span data-stu-id="4be8a-143">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|
|<span data-ttu-id="4be8a-144">displayName</span><span class="sxs-lookup"><span data-stu-id="4be8a-144">displayName</span></span>|<span data-ttu-id="4be8a-145">Строка</span><span class="sxs-lookup"><span data-stu-id="4be8a-145">String</span></span>|<span data-ttu-id="4be8a-146">Имя доли принтера, которую должны отображать клиенты печати.</span><span class="sxs-lookup"><span data-stu-id="4be8a-146">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="4be8a-147">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="4be8a-147">allowAllUsers</span></span>|<span data-ttu-id="4be8a-148">Логический</span><span class="sxs-lookup"><span data-stu-id="4be8a-148">Boolean</span></span>| <span data-ttu-id="4be8a-149">Если это так, всем пользователям и группам будет предоставлен доступ к этой совместной печати.</span><span class="sxs-lookup"><span data-stu-id="4be8a-149">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="4be8a-150">Это замещеет списки разрешенных объектов, определенные свойствами allowedUsers и allowedGroups.</span><span class="sxs-lookup"><span data-stu-id="4be8a-150">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|

## <a name="response"></a><span data-ttu-id="4be8a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4be8a-151">Response</span></span>

<span data-ttu-id="4be8a-152">В случае успешного использования этот метод возвращает код отклика и обновленный объект `200 OK` [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4be8a-152">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4be8a-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="4be8a-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4be8a-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4be8a-154">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="4be8a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4be8a-155">Response</span></span>
<span data-ttu-id="4be8a-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4be8a-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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

