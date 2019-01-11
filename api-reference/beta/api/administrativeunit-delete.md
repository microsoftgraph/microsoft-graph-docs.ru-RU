---
title: Удаление administrativeUnit
description: Удалите administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 7c90fda4bdcbb6a431dbcb4caa6a50a130c7f78b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860055"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="26caf-103">Удаление administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="26caf-103">Delete administrativeUnit</span></span>

> <span data-ttu-id="26caf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="26caf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26caf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26caf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26caf-106">Удалите [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="26caf-106">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26caf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26caf-107">Permissions</span></span>
<span data-ttu-id="26caf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26caf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="26caf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26caf-110">Permission type</span></span>      | <span data-ttu-id="26caf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26caf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26caf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26caf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26caf-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="26caf-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26caf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26caf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26caf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26caf-115">Not supported.</span></span>    |
|<span data-ttu-id="26caf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26caf-116">Application</span></span> | <span data-ttu-id="26caf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26caf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26caf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26caf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="26caf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26caf-119">Request headers</span></span>
| <span data-ttu-id="26caf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="26caf-120">Name</span></span>       | <span data-ttu-id="26caf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="26caf-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="26caf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26caf-122">Authorization</span></span>  | <span data-ttu-id="26caf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26caf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26caf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26caf-125">Request body</span></span>
<span data-ttu-id="26caf-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26caf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26caf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="26caf-127">Response</span></span>

<span data-ttu-id="26caf-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="26caf-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26caf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="26caf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26caf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="26caf-131">Request</span></span>
<span data-ttu-id="26caf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26caf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="26caf-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="26caf-133">Response</span></span>
<span data-ttu-id="26caf-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="26caf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
