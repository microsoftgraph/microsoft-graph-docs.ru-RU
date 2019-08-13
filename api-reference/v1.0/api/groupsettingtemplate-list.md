---
title: Перечисление объектов groupSettingTemplate
description: Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56753600485a015cb85e73b35139edcec8b0f9bc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366360"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="8ab81-104">Перечисление объектов groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8ab81-104">List groupSettingTemplates</span></span>

<span data-ttu-id="8ab81-p102">Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="8ab81-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ab81-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ab81-107">Permissions</span></span>

<span data-ttu-id="8ab81-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ab81-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8ab81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ab81-110">Permission type</span></span>      | <span data-ttu-id="8ab81-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ab81-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ab81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ab81-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8ab81-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ab81-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ab81-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ab81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ab81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ab81-115">Not supported.</span></span>    |
|<span data-ttu-id="8ab81-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ab81-116">Application</span></span> | <span data-ttu-id="8ab81-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ab81-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ab81-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ab81-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8ab81-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8ab81-119">Optional query parameters</span></span>
<span data-ttu-id="8ab81-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8ab81-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="8ab81-121">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ab81-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ab81-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ab81-122">Request headers</span></span>
| <span data-ttu-id="8ab81-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8ab81-123">Name</span></span> | <span data-ttu-id="8ab81-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab81-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="8ab81-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ab81-125">Authorization</span></span>  | <span data-ttu-id="8ab81-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ab81-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ab81-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ab81-128">Request body</span></span>
<span data-ttu-id="8ab81-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ab81-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ab81-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ab81-130">Response</span></span>

<span data-ttu-id="8ab81-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupSettingTemplate](../resources/groupsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ab81-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ab81-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8ab81-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ab81-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ab81-133">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ab81-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ab81-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ab81-135">C#</span><span class="sxs-lookup"><span data-stu-id="8ab81-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ab81-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ab81-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ab81-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8ab81-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ab81-138">Java</span><span class="sxs-lookup"><span data-stu-id="8ab81-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8ab81-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ab81-139">Response</span></span>

<span data-ttu-id="8ab81-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ab81-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
                    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
                    "deletedDateTime": null,
                    "displayName": "Group.Unified",
                    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
                    "values": [
                        {
                            "name": "CustomBlockedWordsList",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "EnableMSStandardBlockedWords",
                            "type": "System.Boolean",
                            "defaultValue": "false",
                            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "ClassificationDescriptions",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
                        }
                    ]
                }
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
