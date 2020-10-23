---
title: 'принтер: Ресторефакторидефаултс'
description: Сброс параметров принтера по умолчанию.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9bae7ed31a9ac73fdda0f576b47129a888190811
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731108"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="a24b4-103">принтер: Ресторефакторидефаултс</span><span class="sxs-lookup"><span data-stu-id="a24b4-103">printer: restoreFactoryDefaults</span></span>

<span data-ttu-id="a24b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a24b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a24b4-105">Восстановите параметры [принтера](../resources/printer.md)в заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="a24b4-105">Restore a [printer](../resources/printer.md)'s settings to the factory settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="a24b4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a24b4-106">Permissions</span></span>
<span data-ttu-id="a24b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a24b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a24b4-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a24b4-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a24b4-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="a24b4-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a24b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a24b4-111">Permission type</span></span> | <span data-ttu-id="a24b4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a24b4-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a24b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a24b4-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a24b4-114">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="a24b4-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a24b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a24b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a24b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a24b4-116">Not Supported.</span></span>|
|<span data-ttu-id="a24b4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a24b4-117">Application</span></span>| <span data-ttu-id="a24b4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a24b4-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a24b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a24b4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/restoreFactoryDefaults
```
## <a name="request-headers"></a><span data-ttu-id="a24b4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a24b4-120">Request headers</span></span>
| <span data-ttu-id="a24b4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a24b4-121">Name</span></span>          | <span data-ttu-id="a24b4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a24b4-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a24b4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a24b4-123">Authorization</span></span> | <span data-ttu-id="a24b4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a24b4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a24b4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a24b4-126">Request body</span></span>
<span data-ttu-id="a24b4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a24b4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a24b4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a24b4-128">Response</span></span>
<span data-ttu-id="a24b4-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a24b4-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a24b4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a24b4-131">Example</span></span>
<span data-ttu-id="a24b4-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a24b4-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="a24b4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a24b4-133">Request</span></span>
<span data-ttu-id="a24b4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a24b4-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printer-restorefactorydefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/restoreFactoryDefaults
```

### <a name="response"></a><span data-ttu-id="a24b4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a24b4-135">Response</span></span>
<span data-ttu-id="a24b4-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a24b4-136">The following is an example of the response.</span></span> 
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
