---
title: Обновление домена
description: Обновление свойств объекта домена.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 07e1e78a43902b846e070523802eeb128217f953
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861413"
---
# <a name="update-domain"></a><span data-ttu-id="900c9-103">Обновление домена</span><span class="sxs-lookup"><span data-stu-id="900c9-103">Update domain</span></span>

<span data-ttu-id="900c9-104">Обновление свойств объекта домена.</span><span class="sxs-lookup"><span data-stu-id="900c9-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="900c9-105">**Важно!** Можно обновить только проверенные домены.</span><span class="sxs-lookup"><span data-stu-id="900c9-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="900c9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="900c9-106">Permissions</span></span>

<span data-ttu-id="900c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="900c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="900c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="900c9-109">Permission type</span></span>      | <span data-ttu-id="900c9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="900c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="900c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="900c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="900c9-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="900c9-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="900c9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="900c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="900c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="900c9-114">Not supported.</span></span>    |
|<span data-ttu-id="900c9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="900c9-115">Application</span></span> | <span data-ttu-id="900c9-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="900c9-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="900c9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="900c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="900c9-118">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="900c9-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="900c9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="900c9-119">Request headers</span></span>

| <span data-ttu-id="900c9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="900c9-120">Name</span></span>       | <span data-ttu-id="900c9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="900c9-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="900c9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="900c9-122">Authorization</span></span>  | <span data-ttu-id="900c9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="900c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="900c9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="900c9-125">Content-Type</span></span>  | <span data-ttu-id="900c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="900c9-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="900c9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="900c9-127">Request body</span></span>

<span data-ttu-id="900c9-p103">В теле запроса укажите значения для соответствующих полей, которые необходимо обновить. Существующие свойства, не включенные в тело запроса, сохранят имеющиеся значения либо будут пересчитаны на основании изменений других значений свойств. Для повышения производительности включайте только измененные значения.</span><span class="sxs-lookup"><span data-stu-id="900c9-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="900c9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="900c9-131">Response</span></span>

<span data-ttu-id="900c9-132">При успешном выполнении этот метод возвращает код отклика `204 No Content` и не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="900c9-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="900c9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="900c9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="900c9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="900c9-134">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="900c9-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="900c9-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
