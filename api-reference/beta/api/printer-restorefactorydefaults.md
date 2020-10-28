---
title: 'принтер: Ресторефакторидефаултс'
description: Сброс параметров принтера по умолчанию.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c1844a46847bd5a232afd60ff61bd7db0e38df83
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782783"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="61a5a-103">принтер: Ресторефакторидефаултс</span><span class="sxs-lookup"><span data-stu-id="61a5a-103">printer: restoreFactoryDefaults</span></span>

<span data-ttu-id="61a5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61a5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61a5a-105">Восстановите параметры [принтера](../resources/printer.md)в заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="61a5a-105">Restore a [printer](../resources/printer.md)'s settings to the factory settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="61a5a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61a5a-106">Permissions</span></span>
<span data-ttu-id="61a5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="61a5a-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="61a5a-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="61a5a-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="61a5a-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="61a5a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61a5a-111">Permission type</span></span> | <span data-ttu-id="61a5a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61a5a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="61a5a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61a5a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="61a5a-114">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="61a5a-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="61a5a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61a5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61a5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61a5a-116">Not Supported.</span></span>|
|<span data-ttu-id="61a5a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="61a5a-117">Application</span></span>| <span data-ttu-id="61a5a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61a5a-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61a5a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61a5a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/restoreFactoryDefaults
```
## <a name="request-headers"></a><span data-ttu-id="61a5a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61a5a-120">Request headers</span></span>
| <span data-ttu-id="61a5a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="61a5a-121">Name</span></span>          | <span data-ttu-id="61a5a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="61a5a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="61a5a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61a5a-123">Authorization</span></span> | <span data-ttu-id="61a5a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61a5a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61a5a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61a5a-126">Request body</span></span>
<span data-ttu-id="61a5a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61a5a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61a5a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="61a5a-128">Response</span></span>
<span data-ttu-id="61a5a-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="61a5a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61a5a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="61a5a-131">Example</span></span>
<span data-ttu-id="61a5a-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="61a5a-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="61a5a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="61a5a-133">Request</span></span>
<span data-ttu-id="61a5a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61a5a-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="61a5a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="61a5a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-restorefactorydefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/restoreFactoryDefaults
```
# <a name="c"></a>[<span data-ttu-id="61a5a-136">C#</span><span class="sxs-lookup"><span data-stu-id="61a5a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-restorefactorydefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61a5a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61a5a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-restorefactorydefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61a5a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61a5a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-restorefactorydefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61a5a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="61a5a-139">Response</span></span>
<span data-ttu-id="61a5a-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="61a5a-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: restoreFactoryDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
