---
title: Обновление printSettings
description: Обновление параметров для клиента для службы универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2d68bed903409fcc20b333e95245e8e15764b348
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787617"
---
# <a name="update-printsettings"></a><span data-ttu-id="df80b-103">Обновление printSettings</span><span class="sxs-lookup"><span data-stu-id="df80b-103">Update printSettings</span></span>
<span data-ttu-id="df80b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df80b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="df80b-105">Обновление параметров для клиента для службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="df80b-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="df80b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df80b-106">Permissions</span></span>
<span data-ttu-id="df80b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df80b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="df80b-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="df80b-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="df80b-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="df80b-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="df80b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df80b-111">Permission type</span></span> | <span data-ttu-id="df80b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df80b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="df80b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df80b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="df80b-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df80b-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="df80b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df80b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df80b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df80b-116">Not Supported.</span></span>|
|<span data-ttu-id="df80b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df80b-117">Application</span></span>|<span data-ttu-id="df80b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df80b-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df80b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df80b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/settings
```

## <a name="request-headers"></a><span data-ttu-id="df80b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df80b-120">Request headers</span></span>
|<span data-ttu-id="df80b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="df80b-121">Name</span></span>|<span data-ttu-id="df80b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="df80b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="df80b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df80b-123">Authorization</span></span>|<span data-ttu-id="df80b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df80b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="df80b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df80b-126">Content-Type</span></span>|<span data-ttu-id="df80b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df80b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df80b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df80b-129">Request body</span></span>
<span data-ttu-id="df80b-130">В теле запроса укажи значения для соответствующих полей [printSettings,](../resources/printsettings.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="df80b-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="df80b-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="df80b-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="df80b-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="df80b-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="df80b-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="df80b-133">Property</span></span>     | <span data-ttu-id="df80b-134">Тип</span><span class="sxs-lookup"><span data-stu-id="df80b-134">Type</span></span>        | <span data-ttu-id="df80b-135">Описание</span><span class="sxs-lookup"><span data-stu-id="df80b-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df80b-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="df80b-136">documentConversionEnabled</span></span>|<span data-ttu-id="df80b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="df80b-137">Boolean</span></span>|<span data-ttu-id="df80b-138">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="df80b-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="df80b-139">Если преобразование документов включено, служба универсальной печати автоматически преобразует документы в формат, совместимый с принтером (например, XPS в PDF) при необходимости.</span><span class="sxs-lookup"><span data-stu-id="df80b-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="df80b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="df80b-140">Response</span></span>

<span data-ttu-id="df80b-141">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="df80b-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df80b-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="df80b-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df80b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="df80b-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="df80b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="df80b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="df80b-145">C#</span><span class="sxs-lookup"><span data-stu-id="df80b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df80b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df80b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df80b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df80b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df80b-148">Java</span><span class="sxs-lookup"><span data-stu-id="df80b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df80b-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="df80b-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

