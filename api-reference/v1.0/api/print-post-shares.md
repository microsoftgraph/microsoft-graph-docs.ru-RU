---
title: Создание printerShare
description: Создает новую долю принтера для указанного принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f22101ff6a621a48285f8064595916e491eb996d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517512"
---
# <a name="create-printershare"></a><span data-ttu-id="6f341-103">Создание printerShare</span><span class="sxs-lookup"><span data-stu-id="6f341-103">Create printerShare</span></span>
<span data-ttu-id="6f341-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f341-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="6f341-105">Создание нового **принтераShare** для указанного [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="6f341-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f341-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f341-106">Permissions</span></span>
<span data-ttu-id="6f341-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f341-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6f341-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="6f341-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="6f341-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="6f341-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="6f341-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f341-111">Permission type</span></span> | <span data-ttu-id="6f341-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f341-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6f341-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f341-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6f341-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f341-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="6f341-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f341-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f341-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f341-116">Not Supported.</span></span>|
|<span data-ttu-id="6f341-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f341-117">Application</span></span>|<span data-ttu-id="6f341-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f341-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f341-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f341-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares
```

## <a name="request-headers"></a><span data-ttu-id="6f341-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f341-120">Request headers</span></span>
|<span data-ttu-id="6f341-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6f341-121">Name</span></span>|<span data-ttu-id="6f341-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6f341-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f341-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f341-123">Authorization</span></span>|<span data-ttu-id="6f341-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f341-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6f341-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f341-126">Content-Type</span></span>|<span data-ttu-id="6f341-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f341-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f341-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f341-129">Request body</span></span>
<span data-ttu-id="6f341-130">В теле запроса поставляем JSON-представление объекта [printerShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="6f341-130">In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="6f341-131">В следующей таблице показаны свойства, которые можно предоставлять при создании [принтераShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="6f341-131">The following table shows the properties that can be provided when you create the [printerShare](../resources/printershare.md).</span></span>

|<span data-ttu-id="6f341-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f341-132">Property</span></span>|<span data-ttu-id="6f341-133">Тип</span><span class="sxs-lookup"><span data-stu-id="6f341-133">Type</span></span>|<span data-ttu-id="6f341-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6f341-134">Description</span></span>|<span data-ttu-id="6f341-135">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="6f341-135">Required?</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="6f341-136">printer</span><span class="sxs-lookup"><span data-stu-id="6f341-136">printer</span></span>|<span data-ttu-id="6f341-137">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="6f341-137">microsoft.graph.printer</span></span>|<span data-ttu-id="6f341-138">Принтер, с который связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="6f341-138">The printer that this printer share is related to.</span></span> <span data-ttu-id="6f341-139">Используйте `printer@odata.bind` синтаксис, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="6f341-139">Use the `printer@odata.bind` syntax, as shown in the following example.</span></span>|<span data-ttu-id="6f341-140">Да</span><span class="sxs-lookup"><span data-stu-id="6f341-140">Yes</span></span>|
|<span data-ttu-id="6f341-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6f341-141">displayName</span></span>|<span data-ttu-id="6f341-142">Строка</span><span class="sxs-lookup"><span data-stu-id="6f341-142">String</span></span>|<span data-ttu-id="6f341-143">Имя доли принтера, которую должны отображать клиенты печати.</span><span class="sxs-lookup"><span data-stu-id="6f341-143">The name of the printer share that print clients should display.</span></span> <span data-ttu-id="6f341-144">Максимальная разрешенная длина — 50 символов.</span><span class="sxs-lookup"><span data-stu-id="6f341-144">Maximum length allowed is 50 characters.</span></span>|<span data-ttu-id="6f341-145">Да</span><span class="sxs-lookup"><span data-stu-id="6f341-145">Yes</span></span>|
|<span data-ttu-id="6f341-146">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="6f341-146">allowAllUsers</span></span>|<span data-ttu-id="6f341-147">Логический</span><span class="sxs-lookup"><span data-stu-id="6f341-147">Boolean</span></span>|<span data-ttu-id="6f341-148">Если всем пользователям и группам будет предоставлен доступ `true` к этой совместной печати.</span><span class="sxs-lookup"><span data-stu-id="6f341-148">If `true`, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="6f341-149">Это замещеет списки разрешенных объектов, определенные **свойствами allowedUsers** и **allowedGroups.**</span><span class="sxs-lookup"><span data-stu-id="6f341-149">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|<span data-ttu-id="6f341-150">Нет</span><span class="sxs-lookup"><span data-stu-id="6f341-150">No</span></span>|

## <a name="response"></a><span data-ttu-id="6f341-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f341-151">Response</span></span>

<span data-ttu-id="6f341-152">В случае успешного использования этот метод возвращает код отклика и `201 Created` объект [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f341-152">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f341-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="6f341-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f341-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f341-154">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="6f341-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f341-155">Response</span></span>
<span data-ttu-id="6f341-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6f341-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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

