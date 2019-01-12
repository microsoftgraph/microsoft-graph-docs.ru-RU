---
title: Удаление administrativeUnit
description: Удалите administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d225245bc81782924038d09ed58b6a46313d7c98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946849"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="3ec79-103">Удаление administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="3ec79-103">Delete administrativeUnit</span></span>

> <span data-ttu-id="3ec79-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3ec79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ec79-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec79-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ec79-106">Удалите [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="3ec79-106">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ec79-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec79-107">Permissions</span></span>
<span data-ttu-id="3ec79-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ec79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ec79-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec79-110">Permission type</span></span>      | <span data-ttu-id="3ec79-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ec79-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ec79-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ec79-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ec79-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ec79-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ec79-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ec79-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec79-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec79-115">Not supported.</span></span>    |
|<span data-ttu-id="3ec79-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ec79-116">Application</span></span> | <span data-ttu-id="3ec79-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ec79-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ec79-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ec79-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3ec79-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ec79-119">Request headers</span></span>
| <span data-ttu-id="3ec79-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3ec79-120">Name</span></span>       | <span data-ttu-id="3ec79-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec79-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ec79-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ec79-122">Authorization</span></span>  | <span data-ttu-id="3ec79-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ec79-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ec79-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ec79-125">Request body</span></span>
<span data-ttu-id="3ec79-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ec79-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ec79-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec79-127">Response</span></span>

<span data-ttu-id="3ec79-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3ec79-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ec79-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3ec79-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ec79-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec79-131">Request</span></span>
<span data-ttu-id="3ec79-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ec79-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="3ec79-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ec79-133">Response</span></span>
<span data-ttu-id="3ec79-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3ec79-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
