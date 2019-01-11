---
title: Обновление домена
description: Обновление свойств объекта домена.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 7815d86a733d597860ed986b926972e328598f65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843521"
---
# <a name="update-domain"></a><span data-ttu-id="9c2f6-103">Обновление домена</span><span class="sxs-lookup"><span data-stu-id="9c2f6-103">Update domain</span></span>

> <span data-ttu-id="9c2f6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c2f6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c2f6-106">Обновление свойств объекта домена.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-106">Update the properties of domain object.</span></span>

> <span data-ttu-id="9c2f6-107">**Важно!** Можно обновить только проверенные домены.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-107">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c2f6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c2f6-108">Permissions</span></span>

<span data-ttu-id="9c2f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c2f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9c2f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c2f6-111">Permission type</span></span>      | <span data-ttu-id="9c2f6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c2f6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c2f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c2f6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9c2f6-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c2f6-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c2f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c2f6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c2f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-116">Not supported.</span></span>    |
|<span data-ttu-id="9c2f6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c2f6-117">Application</span></span> | <span data-ttu-id="9c2f6-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c2f6-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c2f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c2f6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="9c2f6-120">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c2f6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c2f6-121">Request headers</span></span>

| <span data-ttu-id="9c2f6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9c2f6-122">Name</span></span>       | <span data-ttu-id="9c2f6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9c2f6-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9c2f6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c2f6-124">Authorization</span></span>  | <span data-ttu-id="9c2f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c2f6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c2f6-127">Content-Type</span></span>  | <span data-ttu-id="9c2f6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9c2f6-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c2f6-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c2f6-129">Request body</span></span>

<span data-ttu-id="9c2f6-p104">В теле запроса укажите значения для соответствующих полей, которые необходимо обновить. Существующие свойства, не включенные в тело запроса, сохранят имеющиеся значения либо будут пересчитаны на основании изменений других значений свойств. Для повышения производительности включайте только измененные значения.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-p104">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="9c2f6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c2f6-133">Response</span></span>

<span data-ttu-id="9c2f6-134">При успешном выполнении этот метод возвращает код отклика `204 No Content` и не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="9c2f6-134">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c2f6-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9c2f6-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c2f6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c2f6-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="9c2f6-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c2f6-137">Response</span></span>

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
