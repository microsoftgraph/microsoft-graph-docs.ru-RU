---
title: Перечисление schemaExtensions
description: 'Получение списка объектов schemaExtension, созданных любыми приложениями, которыми владеет текущий клиент (которые можно '
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 69eb46efe0a190d3bbdff9cc3965097bcf4126de
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461162"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="10673-103">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="10673-103">List schemaExtensions</span></span>

<span data-ttu-id="10673-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10673-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10673-105">Получение списка объектов [schemaExtension](../resources/schemaextension.md) , созданных всеми приложениями, которыми вы владеете в текущем клиенте (которая может быть **разработкой**, **доступной**или **устаревшей**), а также всеми другими расширениями схемы, принадлежащими другим приложениям, которые помечены как **Доступные**.</span><span class="sxs-lookup"><span data-stu-id="10673-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

> <span data-ttu-id="10673-106">**Примечание:** Список также будет содержать определения расширений схемы (помеченные как `Available` ), созданные другими разработчиками из других клиентов.</span><span class="sxs-lookup"><span data-stu-id="10673-106">**Note:** The list will also contain schema extension definitions (marked as `Available`) created by other developers from other tenants.</span></span> <span data-ttu-id="10673-107">Это отличается от других API-интерфейсов, возвращающих только данные определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="10673-107">This is different from other APIs that only return tenant-specific data.</span></span> <span data-ttu-id="10673-108">Данные расширения, созданные на основе определений расширений схемы, зависят от клиента и доступны только для приложений, которым явно предоставлено разрешение.</span><span class="sxs-lookup"><span data-stu-id="10673-108">Extension data created based on schema extension definitions is tenant-specific and can only be accessed by apps explicitly granted permission.</span></span> 

## <a name="permissions"></a><span data-ttu-id="10673-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10673-109">Permissions</span></span>
<span data-ttu-id="10673-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10673-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="10673-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10673-112">Permission type</span></span>      | <span data-ttu-id="10673-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10673-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10673-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10673-114">Delegated (work or school account)</span></span> | <span data-ttu-id="10673-115">User. Read, Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="10673-115">User.Read, Application.Read.All</span></span>  |
|<span data-ttu-id="10673-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10673-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10673-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10673-117">Not supported.</span></span>    |
|<span data-ttu-id="10673-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="10673-118">Application</span></span> | <span data-ttu-id="10673-119">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="10673-119">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10673-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10673-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10673-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10673-121">Optional query parameters</span></span>
<span data-ttu-id="10673-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10673-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10673-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10673-123">Request headers</span></span>
| <span data-ttu-id="10673-124">Имя</span><span class="sxs-lookup"><span data-stu-id="10673-124">Name</span></span>      |<span data-ttu-id="10673-125">Описание</span><span class="sxs-lookup"><span data-stu-id="10673-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10673-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10673-126">Authorization</span></span>  | <span data-ttu-id="10673-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10673-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10673-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10673-129">Content-Type</span></span>   | <span data-ttu-id="10673-130">application/json</span><span class="sxs-lookup"><span data-stu-id="10673-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="10673-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10673-131">Request body</span></span>
<span data-ttu-id="10673-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10673-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10673-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="10673-133">Response</span></span>

<span data-ttu-id="10673-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [schemaExtension](../resources/schemaextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10673-134">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10673-135">Пример</span><span class="sxs-lookup"><span data-stu-id="10673-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10673-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="10673-136">Request</span></span>
<span data-ttu-id="10673-137">В приведенном ниже примере показано, как просмотреть все доступные расширения для конкретного объекта, выполнив фильтрацию по его уникальному **идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="10673-137">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="10673-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="10673-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="10673-139">C#</span><span class="sxs-lookup"><span data-stu-id="10673-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10673-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10673-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10673-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10673-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10673-142">Java</span><span class="sxs-lookup"><span data-stu-id="10673-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextensions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="10673-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="10673-143">Response</span></span>
<span data-ttu-id="10673-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10673-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
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
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="10673-147">См. также</span><span class="sxs-lookup"><span data-stu-id="10673-147">See also</span></span>

- [<span data-ttu-id="10673-148">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="10673-148">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="10673-149">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="10673-149">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
