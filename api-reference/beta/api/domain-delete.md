---
title: Удаление домена
description: Удаление домена из клиента.
ms.openlocfilehash: 2ed3772d767099e8ccd7fd5453c7a8231c9ea96c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078220"
---
# <a name="delete-domain"></a><span data-ttu-id="9b391-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="9b391-103">Delete domain</span></span>

> <span data-ttu-id="9b391-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b391-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b391-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b391-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b391-106">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="9b391-106">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="9b391-107">**Важные:** Удаленные домены, восстановить невозможно.</span><span class="sxs-lookup"><span data-stu-id="9b391-107">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b391-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b391-108">Permissions</span></span>

<span data-ttu-id="9b391-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b391-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9b391-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b391-111">Permission type</span></span>      | <span data-ttu-id="9b391-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b391-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b391-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b391-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9b391-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9b391-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9b391-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b391-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b391-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b391-116">Not supported.</span></span>    |
|<span data-ttu-id="9b391-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b391-117">Application</span></span> | <span data-ttu-id="9b391-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b391-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b391-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b391-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="9b391-120">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="9b391-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b391-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b391-121">Request headers</span></span>

| <span data-ttu-id="9b391-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9b391-122">Name</span></span>       | <span data-ttu-id="9b391-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9b391-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b391-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b391-124">Authorization</span></span>  | <span data-ttu-id="9b391-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b391-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b391-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b391-127">Content-Type</span></span>  | <span data-ttu-id="9b391-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9b391-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b391-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b391-129">Request body</span></span>

<span data-ttu-id="9b391-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b391-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b391-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b391-131">Response</span></span>

<span data-ttu-id="9b391-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="9b391-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b391-134">Пример</span><span class="sxs-lookup"><span data-stu-id="9b391-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b391-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b391-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="9b391-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b391-136">Response</span></span>

<span data-ttu-id="9b391-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b391-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->