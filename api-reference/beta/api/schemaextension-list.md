---
title: Перечисление schemaExtensions
description: 'Ознакомьтесь со списком schemaExtension объекты, созданные им владеете в текущем клиентов (который может быть любой приложений '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 21e9cb1d202bd76abd71860b14a8c58856132ba1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945169"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="91370-103">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="91370-103">List schemaExtensions</span></span>

> <span data-ttu-id="91370-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91370-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91370-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91370-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91370-106">Получение списка объектов [schemaExtension](../resources/schemaextension.md), созданных любыми приложениями, которыми вы владеете в текущем клиенте (они могут иметь состояние **InDevelopment**, **Available** или **Deprecated**), и всех других расширений схемы, принадлежащих другим приложениям и отмеченных как **Available**.</span><span class="sxs-lookup"><span data-stu-id="91370-106">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="91370-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91370-107">Permissions</span></span>
<span data-ttu-id="91370-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91370-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="91370-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91370-110">Permission type</span></span>      | <span data-ttu-id="91370-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91370-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91370-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91370-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91370-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91370-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91370-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91370-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91370-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91370-115">Not supported.</span></span>    |
|<span data-ttu-id="91370-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91370-116">Application</span></span> | <span data-ttu-id="91370-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="91370-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91370-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91370-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91370-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91370-119">Optional query parameters</span></span>
<span data-ttu-id="91370-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91370-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91370-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91370-121">Request headers</span></span>
| <span data-ttu-id="91370-122">Имя</span><span class="sxs-lookup"><span data-stu-id="91370-122">Name</span></span>      |<span data-ttu-id="91370-123">Описание</span><span class="sxs-lookup"><span data-stu-id="91370-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91370-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91370-124">Authorization</span></span>  | <span data-ttu-id="91370-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91370-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91370-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91370-127">Content-Type</span></span>   | <span data-ttu-id="91370-128">application/json</span><span class="sxs-lookup"><span data-stu-id="91370-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="91370-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91370-129">Request body</span></span>
<span data-ttu-id="91370-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91370-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91370-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="91370-131">Response</span></span>

<span data-ttu-id="91370-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91370-132">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91370-133">Пример</span><span class="sxs-lookup"><span data-stu-id="91370-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91370-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="91370-134">Request</span></span>
<span data-ttu-id="91370-135">В приведенном ниже примере показано, как искать определенное расширение среди всех доступных расширений путем фильтрации по уникальному **идентификатору** расширения.</span><span class="sxs-lookup"><span data-stu-id="91370-135">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="91370-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="91370-136">Response</span></span>
<span data-ttu-id="91370-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="91370-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="91370-140">См. также</span><span class="sxs-lookup"><span data-stu-id="91370-140">See also</span></span>

- [<span data-ttu-id="91370-141">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="91370-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="91370-142">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="91370-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
