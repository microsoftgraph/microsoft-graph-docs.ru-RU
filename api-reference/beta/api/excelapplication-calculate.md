---
title: 'Приложение: вычисление'
description: Пересчитывает данные во всех открытых в текущий момент книгах Excel.
localization_priority: Normal
ms.openlocfilehash: 3d80fc89c002d7c89fcc5d68920895b9b1fe1c4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818335"
---
# <a name="application-calculate"></a><span data-ttu-id="c1be0-103">Приложение: вычисление</span><span class="sxs-lookup"><span data-stu-id="c1be0-103">Application: calculate</span></span>

> <span data-ttu-id="c1be0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1be0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1be0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1be0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1be0-106">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="c1be0-106">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1be0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1be0-107">Permissions</span></span>
<span data-ttu-id="c1be0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1be0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1be0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1be0-110">Permission type</span></span>      | <span data-ttu-id="c1be0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1be0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1be0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1be0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1be0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1be0-113">Not supported.</span></span>    |
|<span data-ttu-id="c1be0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1be0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1be0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1be0-115">Not supported.</span></span>    |
|<span data-ttu-id="c1be0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1be0-116">Application</span></span> | <span data-ttu-id="c1be0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1be0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1be0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1be0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="c1be0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1be0-119">Request headers</span></span>
| <span data-ttu-id="c1be0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c1be0-120">Name</span></span>       | <span data-ttu-id="c1be0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c1be0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1be0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1be0-122">Authorization</span></span>  | <span data-ttu-id="c1be0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1be0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1be0-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1be0-125">Request body</span></span>
<span data-ttu-id="c1be0-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c1be0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1be0-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="c1be0-127">Parameter</span></span>    | <span data-ttu-id="c1be0-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c1be0-128">Type</span></span>   |<span data-ttu-id="c1be0-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c1be0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1be0-130">calculationType</span><span class="sxs-lookup"><span data-stu-id="c1be0-130">calculationType</span></span>|<span data-ttu-id="c1be0-131">string</span><span class="sxs-lookup"><span data-stu-id="c1be0-131">string</span></span>|<span data-ttu-id="c1be0-132">Указывает тип вычислений для использования.</span><span class="sxs-lookup"><span data-stu-id="c1be0-132">Specifies the calculation type to use.</span></span>  <span data-ttu-id="c1be0-133">Возможные значения: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="c1be0-133">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="c1be0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1be0-134">Response</span></span>

<span data-ttu-id="c1be0-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c1be0-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1be0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c1be0-137">Example</span></span>
<span data-ttu-id="c1be0-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c1be0-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1be0-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1be0-139">Request</span></span>
<span data-ttu-id="c1be0-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1be0-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="c1be0-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1be0-141">Response</span></span>
<span data-ttu-id="c1be0-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1be0-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
