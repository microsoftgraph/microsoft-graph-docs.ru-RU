---
title: Перечисление schemaExtensions
description: 'Ознакомьтесь со списком schemaExtension объекты, созданные им владеете в текущем клиентов (который может быть любой приложений '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a320cc0261c40ee8b87dcc658c6ca146d77190e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529161"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="9e72c-103">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="9e72c-103">List schemaExtensions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e72c-104">Получение списка объектов [schemaExtension](../resources/schemaextension.md), созданных любыми приложениями, которыми вы владеете в текущем клиенте (они могут иметь состояние **InDevelopment**, **Available** или **Deprecated**), и всех других расширений схемы, принадлежащих другим приложениям и отмеченных как **Available**.</span><span class="sxs-lookup"><span data-stu-id="9e72c-104">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9e72c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e72c-105">Permissions</span></span>
<span data-ttu-id="9e72c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e72c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9e72c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e72c-108">Permission type</span></span>      | <span data-ttu-id="9e72c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e72c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e72c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e72c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e72c-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e72c-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e72c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e72c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e72c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e72c-113">Not supported.</span></span>    |
|<span data-ttu-id="9e72c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e72c-114">Application</span></span> | <span data-ttu-id="9e72c-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e72c-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e72c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e72c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e72c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e72c-117">Optional query parameters</span></span>
<span data-ttu-id="9e72c-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9e72c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e72c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e72c-119">Request headers</span></span>
| <span data-ttu-id="9e72c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9e72c-120">Name</span></span>      |<span data-ttu-id="9e72c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9e72c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e72c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e72c-122">Authorization</span></span>  | <span data-ttu-id="9e72c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e72c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e72c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e72c-125">Content-Type</span></span>   | <span data-ttu-id="9e72c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e72c-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e72c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e72c-127">Request body</span></span>
<span data-ttu-id="9e72c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e72c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e72c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e72c-129">Response</span></span>

<span data-ttu-id="9e72c-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9e72c-130">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e72c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e72c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e72c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e72c-132">Request</span></span>
<span data-ttu-id="9e72c-133">В приведенном ниже примере показано, как искать определенное расширение среди всех доступных расширений путем фильтрации по уникальному **идентификатору** расширения.</span><span class="sxs-lookup"><span data-stu-id="9e72c-133">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="9e72c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e72c-134">Response</span></span>
<span data-ttu-id="9e72c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9e72c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9e72c-138">См. также</span><span class="sxs-lookup"><span data-stu-id="9e72c-138">See also</span></span>

- [<span data-ttu-id="9e72c-139">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9e72c-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9e72c-140">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="9e72c-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
