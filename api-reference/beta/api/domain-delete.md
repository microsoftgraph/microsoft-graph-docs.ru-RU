---
title: Удаление домена
description: Удаление домена из клиента.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b17d8fea23b48cae8ed3227952fb952297a9aaa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513209"
---
# <a name="delete-domain"></a><span data-ttu-id="d6984-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="d6984-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6984-104">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="d6984-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="d6984-105">**Важные:** Удаленные домены, восстановить невозможно.</span><span class="sxs-lookup"><span data-stu-id="d6984-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6984-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6984-106">Permissions</span></span>

<span data-ttu-id="d6984-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6984-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6984-109">Permission type</span></span>      | <span data-ttu-id="d6984-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6984-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6984-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6984-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d6984-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6984-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6984-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6984-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6984-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6984-114">Not supported.</span></span>    |
|<span data-ttu-id="d6984-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6984-115">Application</span></span> | <span data-ttu-id="d6984-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6984-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6984-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6984-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="d6984-118">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="d6984-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6984-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6984-119">Request headers</span></span>

| <span data-ttu-id="d6984-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d6984-120">Name</span></span>       | <span data-ttu-id="d6984-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d6984-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d6984-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6984-122">Authorization</span></span>  | <span data-ttu-id="d6984-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6984-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6984-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6984-125">Content-Type</span></span>  | <span data-ttu-id="d6984-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6984-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6984-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6984-127">Request body</span></span>

<span data-ttu-id="d6984-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6984-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6984-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6984-129">Response</span></span>

<span data-ttu-id="d6984-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="d6984-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6984-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d6984-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6984-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6984-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="d6984-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6984-134">Response</span></span>

<span data-ttu-id="d6984-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6984-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
