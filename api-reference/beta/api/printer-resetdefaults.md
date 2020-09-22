---
title: 'принтер: Ресетдефаултс'
description: Сброс параметров принтера по умолчанию.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 371c76738833eeabfafb68b1b8c6816f831e32ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035622"
---
# <a name="printer-resetdefaults"></a><span data-ttu-id="e710b-103">принтер: Ресетдефаултс</span><span class="sxs-lookup"><span data-stu-id="e710b-103">printer: resetDefaults</span></span>

<span data-ttu-id="e710b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e710b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e710b-105">Сброс параметров [принтера](../resources/printer.md)по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e710b-105">Reset a [printer](../resources/printer.md)'s default settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="e710b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e710b-106">Permissions</span></span>
<span data-ttu-id="e710b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e710b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e710b-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e710b-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="e710b-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="e710b-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e710b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e710b-111">Permission type</span></span> | <span data-ttu-id="e710b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e710b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e710b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e710b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e710b-114">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="e710b-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="e710b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e710b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e710b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e710b-116">Not Supported.</span></span>|
|<span data-ttu-id="e710b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e710b-117">Application</span></span>| <span data-ttu-id="e710b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e710b-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e710b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e710b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/resetDefaults
```
## <a name="request-headers"></a><span data-ttu-id="e710b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e710b-120">Request headers</span></span>
| <span data-ttu-id="e710b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e710b-121">Name</span></span>          | <span data-ttu-id="e710b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e710b-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e710b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e710b-123">Authorization</span></span> | <span data-ttu-id="e710b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e710b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e710b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e710b-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e710b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e710b-127">Response</span></span>
<span data-ttu-id="e710b-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e710b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e710b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e710b-130">Example</span></span>
<span data-ttu-id="e710b-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e710b-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e710b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e710b-132">Request</span></span>
<span data-ttu-id="e710b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e710b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e710b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e710b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-resetdefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/resetDefaults
```
# <a name="c"></a>[<span data-ttu-id="e710b-135">C#</span><span class="sxs-lookup"><span data-stu-id="e710b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-resetdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e710b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e710b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-resetdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e710b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e710b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-resetdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e710b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e710b-138">Response</span></span>
<span data-ttu-id="e710b-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e710b-139">The following is an example of the response.</span></span> 
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
  "description": "printer: resetDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


