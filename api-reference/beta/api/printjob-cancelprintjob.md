---
title: 'printJob: Канцелпринтжоб'
description: Отмена задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 327ad3d974429f2bbf6482236b4850bbd68db9f9
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896194"
---
# <a name="printjob-cancelprintjob"></a><span data-ttu-id="85179-103">printJob: Канцелпринтжоб</span><span class="sxs-lookup"><span data-stu-id="85179-103">printJob: cancelPrintJob</span></span>

<span data-ttu-id="85179-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85179-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85179-105">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="85179-105">Cancel a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="85179-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85179-106">Permissions</span></span>
<span data-ttu-id="85179-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="85179-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="85179-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="85179-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85179-110">Permission type</span></span> | <span data-ttu-id="85179-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85179-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="85179-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85179-112">Delegated (work or school account)</span></span>| <span data-ttu-id="85179-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="85179-113">Users.Read.All</span></span> |
|<span data-ttu-id="85179-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85179-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85179-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85179-115">Not Supported.</span></span>|
|<span data-ttu-id="85179-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="85179-116">Application</span></span>|<span data-ttu-id="85179-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85179-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85179-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85179-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancelPrintJob
```
## <a name="request-headers"></a><span data-ttu-id="85179-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85179-119">Request headers</span></span>
| <span data-ttu-id="85179-120">Имя</span><span class="sxs-lookup"><span data-stu-id="85179-120">Name</span></span>          | <span data-ttu-id="85179-121">Описание</span><span class="sxs-lookup"><span data-stu-id="85179-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="85179-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85179-122">Authorization</span></span> | <span data-ttu-id="85179-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85179-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85179-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85179-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="85179-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="85179-126">Response</span></span>
<span data-ttu-id="85179-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85179-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85179-129">Пример</span><span class="sxs-lookup"><span data-stu-id="85179-129">Example</span></span>
<span data-ttu-id="85179-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="85179-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85179-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="85179-131">Request</span></span>
<span data-ttu-id="85179-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85179-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "printjob-cancelprintjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancelPrintJob
```

##### <a name="response"></a><span data-ttu-id="85179-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="85179-133">Response</span></span>
<span data-ttu-id="85179-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="85179-134">The following is an example of the response.</span></span> 
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
  "description": "printJob: cancelPrintJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->