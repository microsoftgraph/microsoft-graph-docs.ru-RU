---
title: Обновление printSettings
description: Обновление параметров на всем клиенте для службы универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 232296196ccdee3124d79e0347dde20f5f8aeee8
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873579"
---
# <a name="update-printsettings"></a><span data-ttu-id="a0e1e-103">Обновление printSettings</span><span class="sxs-lookup"><span data-stu-id="a0e1e-103">Update printSettings</span></span>

<span data-ttu-id="a0e1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0e1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0e1e-105">Обновление параметров на всем клиенте для службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0e1e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0e1e-106">Permissions</span></span>
<span data-ttu-id="a0e1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0e1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a0e1e-109">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть активная подписка универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a0e1e-110">Пользователь, выписав его, должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a0e1e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a0e1e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0e1e-111">Permission type</span></span> | <span data-ttu-id="a0e1e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0e1e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a0e1e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0e1e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a0e1e-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0e1e-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="a0e1e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0e1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0e1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-116">Not Supported.</span></span>|
|<span data-ttu-id="a0e1e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a0e1e-117">Application</span></span>|<span data-ttu-id="a0e1e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0e1e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0e1e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="a0e1e-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0e1e-120">Optional request headers</span></span>
| <span data-ttu-id="a0e1e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a0e1e-121">Name</span></span>       | <span data-ttu-id="a0e1e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a0e1e-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a0e1e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0e1e-123">Authorization</span></span> | <span data-ttu-id="a0e1e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0e1e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0e1e-126">Content-type</span></span>  | <span data-ttu-id="a0e1e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0e1e-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0e1e-129">Request body</span></span>
<span data-ttu-id="a0e1e-130">В теле запроса укажите значения для соответствующих полей [printSettings,](../resources/printsettings.md) которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="a0e1e-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a0e1e-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a0e1e-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0e1e-133">Property</span></span>     | <span data-ttu-id="a0e1e-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a0e1e-134">Type</span></span>        | <span data-ttu-id="a0e1e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a0e1e-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0e1e-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="a0e1e-136">documentConversionEnabled</span></span>|<span data-ttu-id="a0e1e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0e1e-137">Boolean</span></span>|<span data-ttu-id="a0e1e-138">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="a0e1e-139">Если преобразование документов включено, при необходимости служба универсальной печати автоматически преобразует документы в формат, совместимый с принтером (например, XPS в PDF).</span><span class="sxs-lookup"><span data-stu-id="a0e1e-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="a0e1e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0e1e-140">Response</span></span>
<span data-ttu-id="a0e1e-141">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0e1e-142">Пример</span><span class="sxs-lookup"><span data-stu-id="a0e1e-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0e1e-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0e1e-143">Request</span></span>
<span data-ttu-id="a0e1e-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0e1e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0e1e-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_settings"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="a0e1e-146">C#</span><span class="sxs-lookup"><span data-stu-id="a0e1e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0e1e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0e1e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0e1e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0e1e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0e1e-149">Java</span><span class="sxs-lookup"><span data-stu-id="a0e1e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a0e1e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0e1e-150">Response</span></span>
<span data-ttu-id="a0e1e-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a0e1e-151">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
} -->
```http
HTTP/1.1 204 NoContent
Content-length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
