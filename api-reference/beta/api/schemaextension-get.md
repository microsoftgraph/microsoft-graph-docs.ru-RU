---
title: Получение schemaExtension
description: Получение свойств указанного определения schemaExtension.
ms.openlocfilehash: 32376d6afd0d6171362db1978b708610d9f4d056
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080611"
---
# <a name="get-schemaextension"></a><span data-ttu-id="6775f-103">Получение schemaExtension</span><span class="sxs-lookup"><span data-stu-id="6775f-103">Get schemaExtension</span></span>

> <span data-ttu-id="6775f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6775f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6775f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6775f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6775f-106">Получение свойств указанного определения [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="6775f-106">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="6775f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6775f-107">Permissions</span></span>
<span data-ttu-id="6775f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6775f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6775f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6775f-110">Permission type</span></span>      | <span data-ttu-id="6775f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6775f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6775f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6775f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6775f-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6775f-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6775f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6775f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6775f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6775f-115">Not supported.</span></span>    |
|<span data-ttu-id="6775f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6775f-116">Application</span></span> | <span data-ttu-id="6775f-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6775f-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6775f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6775f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6775f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6775f-119">Optional query parameters</span></span>
<span data-ttu-id="6775f-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6775f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6775f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6775f-121">Request headers</span></span>
| <span data-ttu-id="6775f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6775f-122">Name</span></span>      |<span data-ttu-id="6775f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6775f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6775f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6775f-124">Authorization</span></span>  | <span data-ttu-id="6775f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6775f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6775f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6775f-127">Content-Type</span></span>   | <span data-ttu-id="6775f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6775f-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6775f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6775f-129">Request body</span></span>
<span data-ttu-id="6775f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6775f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6775f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6775f-131">Response</span></span>

<span data-ttu-id="6775f-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6775f-132">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6775f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6775f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6775f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6775f-134">Request</span></span>
<span data-ttu-id="6775f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6775f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="6775f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6775f-136">Response</span></span>
<span data-ttu-id="6775f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6775f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="6775f-140">См. также</span><span class="sxs-lookup"><span data-stu-id="6775f-140">See also</span></span>

- [<span data-ttu-id="6775f-141">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="6775f-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6775f-142">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="6775f-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->