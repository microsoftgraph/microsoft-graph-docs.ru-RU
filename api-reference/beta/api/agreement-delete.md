---
title: Удаление соглашения
description: Удаление объекта соглашения.
ms.openlocfilehash: 919fc628e5f8ff9b6c016e085671f47ed6d56a5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077622"
---
# <a name="delete-agreement"></a><span data-ttu-id="44fb3-103">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="44fb3-103">Delete agreement</span></span>

> <span data-ttu-id="44fb3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44fb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44fb3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44fb3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44fb3-106">Удаление объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="44fb3-106">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="44fb3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44fb3-107">Permissions</span></span>
<span data-ttu-id="44fb3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44fb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44fb3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44fb3-110">Permission type</span></span>                        | <span data-ttu-id="44fb3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44fb3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="44fb3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44fb3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="44fb3-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44fb3-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="44fb3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44fb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44fb3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44fb3-115">Not supported.</span></span> |
|<span data-ttu-id="44fb3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44fb3-116">Application</span></span>                            | <span data-ttu-id="44fb3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44fb3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44fb3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44fb3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="44fb3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44fb3-119">Request headers</span></span>
| <span data-ttu-id="44fb3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="44fb3-120">Name</span></span>         | <span data-ttu-id="44fb3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="44fb3-121">Type</span></span>        | <span data-ttu-id="44fb3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="44fb3-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="44fb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44fb3-123">Authorization</span></span> | <span data-ttu-id="44fb3-124">string</span><span class="sxs-lookup"><span data-stu-id="44fb3-124">string</span></span> | <span data-ttu-id="44fb3-125">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="44fb3-125">Bearer \{token\}.</span></span> <span data-ttu-id="44fb3-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="44fb3-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44fb3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44fb3-127">Request body</span></span>
<span data-ttu-id="44fb3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44fb3-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="44fb3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="44fb3-129">Response</span></span>
<span data-ttu-id="44fb3-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="44fb3-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44fb3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="44fb3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44fb3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="44fb3-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="44fb3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="44fb3-134">Response</span></span>
><span data-ttu-id="44fb3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44fb3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
