---
title: Удаление домена
description: Удаление домена из клиента.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 2ad4a8b66861c7f9e461e49004be3722e841bef0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887614"
---
# <a name="delete-domain"></a><span data-ttu-id="1d692-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="1d692-103">Delete domain</span></span>

> <span data-ttu-id="1d692-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d692-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d692-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d692-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d692-106">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="1d692-106">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="1d692-107">**Важные:** Удаленные домены, восстановить невозможно.</span><span class="sxs-lookup"><span data-stu-id="1d692-107">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d692-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d692-108">Permissions</span></span>

<span data-ttu-id="1d692-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d692-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d692-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d692-111">Permission type</span></span>      | <span data-ttu-id="1d692-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d692-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d692-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d692-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1d692-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d692-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d692-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d692-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d692-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d692-116">Not supported.</span></span>    |
|<span data-ttu-id="1d692-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d692-117">Application</span></span> | <span data-ttu-id="1d692-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d692-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d692-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d692-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="1d692-120">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="1d692-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d692-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d692-121">Request headers</span></span>

| <span data-ttu-id="1d692-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1d692-122">Name</span></span>       | <span data-ttu-id="1d692-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1d692-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d692-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d692-124">Authorization</span></span>  | <span data-ttu-id="1d692-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d692-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d692-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d692-127">Content-Type</span></span>  | <span data-ttu-id="1d692-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1d692-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d692-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d692-129">Request body</span></span>

<span data-ttu-id="1d692-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d692-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d692-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d692-131">Response</span></span>

<span data-ttu-id="1d692-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="1d692-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d692-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1d692-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d692-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d692-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="1d692-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d692-136">Response</span></span>

<span data-ttu-id="1d692-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d692-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
