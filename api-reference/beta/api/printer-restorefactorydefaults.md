---
title: 'принтер: restoreFactoryDefaults'
description: Сброс параметров по умолчанию принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 87e31568dcbe17ec4bd5e3017e852fb17c6f9989
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786464"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="ad2f0-103">принтер: restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="ad2f0-103">printer: restoreFactoryDefaults</span></span>

<span data-ttu-id="ad2f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad2f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad2f0-105">Восстановление [параметров](../resources/printer.md)по умолчанию принтера до значений, заданных производителем.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-105">Restore a [printer](../resources/printer.md)'s default settings to the values specified by the manufacturer.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad2f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad2f0-106">Permissions</span></span>
<span data-ttu-id="ad2f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad2f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ad2f0-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="ad2f0-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="ad2f0-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ad2f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad2f0-111">Permission type</span></span> | <span data-ttu-id="ad2f0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad2f0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ad2f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad2f0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ad2f0-114">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ad2f0-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="ad2f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad2f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad2f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-116">Not Supported.</span></span>|
|<span data-ttu-id="ad2f0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad2f0-117">Application</span></span>| <span data-ttu-id="ad2f0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad2f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad2f0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/restoreFactoryDefaults
```
## <a name="request-headers"></a><span data-ttu-id="ad2f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad2f0-120">Request headers</span></span>
| <span data-ttu-id="ad2f0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ad2f0-121">Name</span></span>          | <span data-ttu-id="ad2f0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ad2f0-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ad2f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad2f0-123">Authorization</span></span> | <span data-ttu-id="ad2f0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad2f0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad2f0-126">Request body</span></span>
<span data-ttu-id="ad2f0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad2f0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad2f0-128">Response</span></span>
<span data-ttu-id="ad2f0-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad2f0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ad2f0-131">Example</span></span>
<span data-ttu-id="ad2f0-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="ad2f0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad2f0-133">Request</span></span>
<span data-ttu-id="ad2f0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad2f0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad2f0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-restorefactorydefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/restoreFactoryDefaults
```
# <a name="c"></a>[<span data-ttu-id="ad2f0-136">C#</span><span class="sxs-lookup"><span data-stu-id="ad2f0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-restorefactorydefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad2f0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad2f0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-restorefactorydefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad2f0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad2f0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-restorefactorydefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad2f0-139">Java</span><span class="sxs-lookup"><span data-stu-id="ad2f0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-restorefactorydefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad2f0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad2f0-140">Response</span></span>
<span data-ttu-id="ad2f0-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad2f0-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
