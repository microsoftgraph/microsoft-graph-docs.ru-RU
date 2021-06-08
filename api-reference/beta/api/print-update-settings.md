---
title: Обновление printSettings
description: Обновление параметров для клиента для службы универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 000e8513bd4c1bfff047d50dad1fd8d1dc7fa4fa
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787620"
---
# <a name="update-printsettings"></a><span data-ttu-id="d0913-103">Обновление printSettings</span><span class="sxs-lookup"><span data-stu-id="d0913-103">Update printSettings</span></span>

<span data-ttu-id="d0913-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0913-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0913-105">Обновление параметров для клиента для службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="d0913-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0913-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0913-106">Permissions</span></span>
<span data-ttu-id="d0913-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d0913-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="d0913-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="d0913-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="d0913-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="d0913-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0913-111">Permission type</span></span> | <span data-ttu-id="d0913-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0913-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d0913-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0913-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d0913-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0913-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="d0913-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0913-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0913-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0913-116">Not Supported.</span></span>|
|<span data-ttu-id="d0913-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0913-117">Application</span></span>|<span data-ttu-id="d0913-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0913-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0913-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0913-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="d0913-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0913-120">Optional request headers</span></span>
| <span data-ttu-id="d0913-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d0913-121">Name</span></span>       | <span data-ttu-id="d0913-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d0913-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d0913-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0913-123">Authorization</span></span> | <span data-ttu-id="d0913-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0913-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0913-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0913-126">Content-type</span></span>  | <span data-ttu-id="d0913-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0913-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0913-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0913-129">Request body</span></span>
<span data-ttu-id="d0913-130">В теле запроса укажи значения для соответствующих полей [printSettings,](../resources/printsettings.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="d0913-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="d0913-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="d0913-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d0913-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d0913-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0913-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0913-133">Property</span></span>     | <span data-ttu-id="d0913-134">Тип</span><span class="sxs-lookup"><span data-stu-id="d0913-134">Type</span></span>        | <span data-ttu-id="d0913-135">Описание</span><span class="sxs-lookup"><span data-stu-id="d0913-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0913-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="d0913-136">documentConversionEnabled</span></span>|<span data-ttu-id="d0913-137">Логический</span><span class="sxs-lookup"><span data-stu-id="d0913-137">Boolean</span></span>|<span data-ttu-id="d0913-138">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0913-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="d0913-139">Если преобразование документов включено, служба универсальной печати автоматически преобразует документы в формат, совместимый с принтером (например, XPS в PDF) при необходимости.</span><span class="sxs-lookup"><span data-stu-id="d0913-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="d0913-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0913-140">Response</span></span>
<span data-ttu-id="d0913-141">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="d0913-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0913-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d0913-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0913-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0913-143">Request</span></span>
<span data-ttu-id="d0913-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0913-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0913-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0913-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d0913-146">C#</span><span class="sxs-lookup"><span data-stu-id="d0913-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0913-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0913-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0913-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0913-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0913-149">Java</span><span class="sxs-lookup"><span data-stu-id="d0913-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0913-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0913-150">Response</span></span>
<span data-ttu-id="d0913-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d0913-151">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
