---
title: Получение schemaExtension
description: Получение свойств указанного определения schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 70a4fdc5e51a5965098a6b0331a31c200b553ec9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980316"
---
# <a name="get-schemaextension"></a><span data-ttu-id="2d713-103">Получение schemaExtension</span><span class="sxs-lookup"><span data-stu-id="2d713-103">Get schemaExtension</span></span>
<span data-ttu-id="2d713-104">Получение свойств указанного определения [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="2d713-104">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d713-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d713-105">Permissions</span></span>
<span data-ttu-id="2d713-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d713-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2d713-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d713-108">Permission type</span></span>      | <span data-ttu-id="2d713-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d713-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d713-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d713-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d713-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d713-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d713-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d713-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d713-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d713-113">Not supported.</span></span>    |
|<span data-ttu-id="2d713-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d713-114">Application</span></span> | <span data-ttu-id="2d713-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d713-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d713-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d713-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d713-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d713-117">Optional query parameters</span></span>
<span data-ttu-id="2d713-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2d713-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d713-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d713-119">Request headers</span></span>
| <span data-ttu-id="2d713-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2d713-120">Name</span></span>      |<span data-ttu-id="2d713-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2d713-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2d713-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d713-122">Authorization</span></span>  | <span data-ttu-id="2d713-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d713-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d713-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d713-125">Content-Type</span></span>   | <span data-ttu-id="2d713-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d713-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d713-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d713-127">Request body</span></span>
<span data-ttu-id="2d713-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d713-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d713-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d713-129">Response</span></span>

<span data-ttu-id="2d713-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d713-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d713-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2d713-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d713-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d713-132">Request</span></span>
<span data-ttu-id="2d713-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d713-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="2d713-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d713-134">Response</span></span>
<span data-ttu-id="2d713-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2d713-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
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

## <a name="see-also"></a><span data-ttu-id="2d713-138">См. также</span><span class="sxs-lookup"><span data-stu-id="2d713-138">See also</span></span>

- [<span data-ttu-id="2d713-139">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="2d713-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2d713-140">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="2d713-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
