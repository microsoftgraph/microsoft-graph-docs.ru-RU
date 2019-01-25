---
title: 'Приложение: вычисление'
description: Пересчитывает данные во всех открытых в текущий момент книгах Excel.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: f16c858f7e8c9d85dbe8252bde0a791bc325514c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514504"
---
# <a name="application-calculate"></a><span data-ttu-id="a8a68-103">Приложение: вычисление</span><span class="sxs-lookup"><span data-stu-id="a8a68-103">Application: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8a68-104">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="a8a68-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8a68-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8a68-105">Permissions</span></span>
<span data-ttu-id="a8a68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8a68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8a68-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8a68-108">Permission type</span></span>      | <span data-ttu-id="a8a68-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8a68-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8a68-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8a68-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8a68-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8a68-111">Not supported.</span></span>    |
|<span data-ttu-id="a8a68-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8a68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8a68-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8a68-113">Not supported.</span></span>    |
|<span data-ttu-id="a8a68-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8a68-114">Application</span></span> | <span data-ttu-id="a8a68-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8a68-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8a68-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8a68-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="a8a68-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8a68-117">Request headers</span></span>
| <span data-ttu-id="a8a68-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a8a68-118">Name</span></span>       | <span data-ttu-id="a8a68-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a8a68-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8a68-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8a68-120">Authorization</span></span>  | <span data-ttu-id="a8a68-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8a68-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8a68-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8a68-123">Request body</span></span>
<span data-ttu-id="a8a68-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a8a68-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8a68-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="a8a68-125">Parameter</span></span>    | <span data-ttu-id="a8a68-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a8a68-126">Type</span></span>   |<span data-ttu-id="a8a68-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a8a68-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8a68-128">calculationType</span><span class="sxs-lookup"><span data-stu-id="a8a68-128">calculationType</span></span>|<span data-ttu-id="a8a68-129">string</span><span class="sxs-lookup"><span data-stu-id="a8a68-129">string</span></span>|<span data-ttu-id="a8a68-130">Указывает тип вычислений для использования.</span><span class="sxs-lookup"><span data-stu-id="a8a68-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="a8a68-131">Возможные значения: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="a8a68-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="a8a68-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8a68-132">Response</span></span>

<span data-ttu-id="a8a68-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a8a68-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8a68-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a8a68-135">Example</span></span>
<span data-ttu-id="a8a68-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a8a68-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a8a68-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8a68-137">Request</span></span>
<span data-ttu-id="a8a68-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8a68-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a8a68-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8a68-139">Response</span></span>
<span data-ttu-id="a8a68-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8a68-140">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Application: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/excelapplication-calculate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
