---
title: Удаление Таскдефинитион
description: Удаление определения задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 23d7438d573cb0ac8ff17c0a9c100bece71bb68c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091748"
---
# <a name="delete-taskdefinition"></a><span data-ttu-id="48b3a-103">Удаление Таскдефинитион</span><span class="sxs-lookup"><span data-stu-id="48b3a-103">Delete taskDefinition</span></span>

<span data-ttu-id="48b3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48b3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48b3a-105">Удаление объекта **таскдефинитион**.</span><span class="sxs-lookup"><span data-stu-id="48b3a-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="48b3a-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="48b3a-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="48b3a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48b3a-107">Permissions</span></span>
<span data-ttu-id="48b3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48b3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="48b3a-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="48b3a-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="48b3a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48b3a-111">Permission type</span></span> | <span data-ttu-id="48b3a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48b3a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="48b3a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48b3a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="48b3a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48b3a-114">Not supported.</span></span> |
|<span data-ttu-id="48b3a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48b3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48b3a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48b3a-116">Not Supported.</span></span>|
|<span data-ttu-id="48b3a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48b3a-117">Application</span></span>| <span data-ttu-id="48b3a-118">Принттаскдефинитион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="48b3a-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48b3a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48b3a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/taskDefinitions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="48b3a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48b3a-120">Request headers</span></span>
| <span data-ttu-id="48b3a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="48b3a-121">Name</span></span>          | <span data-ttu-id="48b3a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="48b3a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="48b3a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48b3a-123">Authorization</span></span> | <span data-ttu-id="48b3a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48b3a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48b3a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48b3a-126">Request body</span></span>
<span data-ttu-id="48b3a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48b3a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48b3a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="48b3a-128">Response</span></span>
<span data-ttu-id="48b3a-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48b3a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48b3a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="48b3a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="48b3a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="48b3a-132">Request</span></span>
<span data-ttu-id="48b3a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48b3a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_taskdefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19
```

---

### <a name="response"></a><span data-ttu-id="48b3a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="48b3a-134">Response</span></span>
<span data-ttu-id="48b3a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48b3a-135">The following is an example of the response.</span></span>
><span data-ttu-id="48b3a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48b3a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
