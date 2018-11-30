---
title: Обновление synchronizationTemplate
description: Обновление (переопределение) шаблон синхронизации, связанный с заданным приложением.
ms.openlocfilehash: 9862b0a31294448e1b43e8438b76a16d471cb2d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081926"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="4dcf0-103">Обновление synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="4dcf0-103">Update synchronizationTemplate</span></span>

> <span data-ttu-id="4dcf0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dcf0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4dcf0-106">Обновление (переопределение) шаблон синхронизации, связанный с заданным приложением.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-106">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dcf0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4dcf0-107">Permissions</span></span>
<span data-ttu-id="4dcf0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dcf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dcf0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dcf0-110">Permission type</span></span>                        | <span data-ttu-id="4dcf0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dcf0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dcf0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dcf0-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="4dcf0-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dcf0-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4dcf0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dcf0-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4dcf0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-115">Not supported.</span></span>|
|<span data-ttu-id="4dcf0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dcf0-116">Application</span></span>                            |<span data-ttu-id="4dcf0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="4dcf0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dcf0-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="4dcf0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dcf0-119">Request headers</span></span>

| <span data-ttu-id="4dcf0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4dcf0-120">Name</span></span>           | <span data-ttu-id="4dcf0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4dcf0-121">Type</span></span>    | <span data-ttu-id="4dcf0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4dcf0-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4dcf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dcf0-123">Authorization</span></span>  | <span data-ttu-id="4dcf0-124">string</span><span class="sxs-lookup"><span data-stu-id="4dcf0-124">string</span></span>  | <span data-ttu-id="4dcf0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dcf0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dcf0-127">Request body</span></span>

<span data-ttu-id="4dcf0-128">В тексте запроса предоставить к объекту [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) , чтобы заменить существующий шаблон.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="4dcf0-129">Убедитесь, что все свойства.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-129">Make sure all properties are provided.</span></span> <span data-ttu-id="4dcf0-130">Отсутствующие свойства будут удалены.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-130">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="4dcf0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dcf0-131">Response</span></span>

<span data-ttu-id="4dcf0-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="4dcf0-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="4dcf0-134">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="4dcf0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dcf0-135">Request</span></span>
<span data-ttu-id="4dcf0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-136">The following is an example of a request.</span></span> 

><span data-ttu-id="4dcf0-137">**Примечание:** Объект запроса, показанный сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-137">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="4dcf0-138">Включите все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-138">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="4dcf0-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dcf0-139">Response</span></span>
<span data-ttu-id="4dcf0-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4dcf0-140">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->