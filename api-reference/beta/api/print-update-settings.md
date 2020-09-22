---
title: Обновление Принтсеттингс
description: Обновление параметров на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a37b918b083bbc8a1e76eae073f68979dbcdf035
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035907"
---
# <a name="update-printsettings"></a><span data-ttu-id="1af40-103">Обновление Принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="1af40-103">Update printSettings</span></span>

<span data-ttu-id="1af40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1af40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1af40-105">Обновление параметров на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="1af40-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="1af40-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1af40-106">Permissions</span></span>
<span data-ttu-id="1af40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1af40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1af40-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1af40-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="1af40-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="1af40-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="1af40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1af40-111">Permission type</span></span> | <span data-ttu-id="1af40-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1af40-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1af40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1af40-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1af40-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="1af40-114">User.Read</span></span> |
|<span data-ttu-id="1af40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1af40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1af40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af40-116">Not Supported.</span></span>|
|<span data-ttu-id="1af40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1af40-117">Application</span></span>|<span data-ttu-id="1af40-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af40-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1af40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1af40-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="1af40-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1af40-120">Optional request headers</span></span>
| <span data-ttu-id="1af40-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1af40-121">Name</span></span>       | <span data-ttu-id="1af40-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1af40-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1af40-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1af40-123">Authorization</span></span> | <span data-ttu-id="1af40-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1af40-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1af40-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1af40-126">Content-type</span></span>  | <span data-ttu-id="1af40-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1af40-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1af40-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1af40-129">Request body</span></span>
<span data-ttu-id="1af40-130">В тексте запроса укажите значения для соответствующих полей [принтсеттингс](../resources/printsettings.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1af40-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="1af40-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1af40-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1af40-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1af40-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1af40-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="1af40-133">Property</span></span>     | <span data-ttu-id="1af40-134">Тип</span><span class="sxs-lookup"><span data-stu-id="1af40-134">Type</span></span>        | <span data-ttu-id="1af40-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1af40-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1af40-136">документконверсионенаблед</span><span class="sxs-lookup"><span data-stu-id="1af40-136">documentConversionEnabled</span></span>|<span data-ttu-id="1af40-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1af40-137">Boolean</span></span>|<span data-ttu-id="1af40-138">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="1af40-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="1af40-139">Если включено преобразование документов, то при необходимости в универсальной службе печати документы автоматически преобразуются в формат, совместимый с принтером (например, XPS — PDF).</span><span class="sxs-lookup"><span data-stu-id="1af40-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="1af40-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1af40-140">Response</span></span>
<span data-ttu-id="1af40-141">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="1af40-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="1af40-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1af40-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1af40-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="1af40-143">Request</span></span>
<span data-ttu-id="1af40-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1af40-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1af40-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="1af40-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1af40-146">C#</span><span class="sxs-lookup"><span data-stu-id="1af40-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1af40-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1af40-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1af40-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1af40-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1af40-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1af40-149">Response</span></span>
<span data-ttu-id="1af40-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1af40-150">The following is an example of the response.</span></span> 
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


