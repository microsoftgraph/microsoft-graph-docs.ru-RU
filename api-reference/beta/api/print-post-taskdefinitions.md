---
title: Создание Таскдефинитион
description: Создайте новое определение задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 147e1271ee0f5bcd7c04e167e172c48939a4da98
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091717"
---
# <a name="create-taskdefinition"></a><span data-ttu-id="17ec5-103">Создание Таскдефинитион</span><span class="sxs-lookup"><span data-stu-id="17ec5-103">Create taskDefinition</span></span>

<span data-ttu-id="17ec5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17ec5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17ec5-105">Создайте новое определение задачи.</span><span class="sxs-lookup"><span data-stu-id="17ec5-105">Create a new task definition.</span></span>

<span data-ttu-id="17ec5-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="17ec5-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="17ec5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17ec5-107">Permissions</span></span>
<span data-ttu-id="17ec5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17ec5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="17ec5-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="17ec5-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="17ec5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17ec5-111">Permission type</span></span> | <span data-ttu-id="17ec5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17ec5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="17ec5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17ec5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="17ec5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17ec5-114">Not supported.</span></span> |
|<span data-ttu-id="17ec5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17ec5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17ec5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17ec5-116">Not Supported.</span></span>|
|<span data-ttu-id="17ec5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17ec5-117">Application</span></span>| <span data-ttu-id="17ec5-118">Принттаскдефинитион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="17ec5-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17ec5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17ec5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="17ec5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17ec5-120">Request headers</span></span>
| <span data-ttu-id="17ec5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="17ec5-121">Name</span></span>      |<span data-ttu-id="17ec5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="17ec5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17ec5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17ec5-123">Authorization</span></span> | <span data-ttu-id="17ec5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17ec5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17ec5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17ec5-126">Content-type</span></span>  | <span data-ttu-id="17ec5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17ec5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17ec5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17ec5-129">Request body</span></span>
<span data-ttu-id="17ec5-130">В тексте запроса добавьте представление объекта [принттаскдефинитион](../resources/printtaskdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17ec5-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="17ec5-131">Свойства [принттаскдефинитион](../resources/printtaskdefinition.md) **ID** и **createdBy. AppID** задаются автоматически при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="17ec5-131">The [printTaskDefinition](../resources/printtaskdefinition.md)'s **id** and **createdBy.appId** properties are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="17ec5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="17ec5-132">Response</span></span>
<span data-ttu-id="17ec5-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [принттаскдефинитион](../resources/printtaskdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17ec5-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17ec5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="17ec5-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="17ec5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="17ec5-135">Request</span></span>
<span data-ttu-id="17ec5-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17ec5-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "print_create_taskdefinition"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/print/taskDefinitions
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```

---

### <a name="response"></a><span data-ttu-id="17ec5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="17ec5-137">Response</span></span>
<span data-ttu-id="17ec5-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17ec5-138">The following is an example of the response.</span></span>
><span data-ttu-id="17ec5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17ec5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 322

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
