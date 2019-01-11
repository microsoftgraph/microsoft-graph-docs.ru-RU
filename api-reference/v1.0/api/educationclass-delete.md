---
title: Удаление educationClass
description: Удаление класса. Так как класс также является универсальной группой, удаление класса приводит к удалению группы.
localization_priority: Normal
ms.openlocfilehash: 0bb7c6892fed12381b32ac5b4767375ae98d8506
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880313"
---
# <a name="delete-educationclass"></a><span data-ttu-id="7b915-104">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="7b915-104">Delete educationClass</span></span>

<span data-ttu-id="7b915-105">Удаление класса.</span><span class="sxs-lookup"><span data-stu-id="7b915-105">Delete a class.</span></span> <span data-ttu-id="7b915-106">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="7b915-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b915-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b915-107">Permissions</span></span>
<span data-ttu-id="7b915-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b915-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b915-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b915-110">Permission type</span></span>      | <span data-ttu-id="7b915-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b915-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b915-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b915-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="7b915-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b915-113">Not supported.</span></span>  |
|<span data-ttu-id="7b915-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b915-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7b915-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b915-115">Not supported.</span></span>  |
|<span data-ttu-id="7b915-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b915-116">Application</span></span> | <span data-ttu-id="7b915-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b915-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7b915-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b915-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7b915-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b915-119">Request headers</span></span>
| <span data-ttu-id="7b915-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b915-120">Header</span></span>       | <span data-ttu-id="7b915-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7b915-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7b915-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b915-122">Authorization</span></span>  | <span data-ttu-id="7b915-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b915-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b915-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b915-125">Request body</span></span>
<span data-ttu-id="7b915-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b915-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7b915-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b915-127">Response</span></span>
<span data-ttu-id="7b915-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7b915-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b915-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7b915-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b915-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b915-131">Request</span></span>
<span data-ttu-id="7b915-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b915-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="7b915-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b915-133">Response</span></span>
<span data-ttu-id="7b915-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b915-134">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
