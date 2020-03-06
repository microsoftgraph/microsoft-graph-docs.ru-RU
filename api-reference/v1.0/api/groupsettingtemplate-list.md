---
title: Перечисление объектов groupSettingTemplate
description: Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d529d7d012a3bdf15c14fcd01482787ba5656636
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516803"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="c03bb-104">Перечисление объектов groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="c03bb-104">List groupSettingTemplates</span></span>

<span data-ttu-id="c03bb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c03bb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c03bb-p102">Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="c03bb-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c03bb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c03bb-108">Permissions</span></span>

<span data-ttu-id="c03bb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c03bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c03bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c03bb-111">Permission type</span></span>      | <span data-ttu-id="c03bb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c03bb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c03bb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c03bb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c03bb-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c03bb-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c03bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c03bb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c03bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c03bb-116">Not supported.</span></span>    |
|<span data-ttu-id="c03bb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c03bb-117">Application</span></span> | <span data-ttu-id="c03bb-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c03bb-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c03bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c03bb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c03bb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c03bb-120">Optional query parameters</span></span>
<span data-ttu-id="c03bb-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c03bb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="c03bb-122">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c03bb-122">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c03bb-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c03bb-123">Request headers</span></span>
| <span data-ttu-id="c03bb-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c03bb-124">Name</span></span> | <span data-ttu-id="c03bb-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c03bb-125">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="c03bb-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c03bb-126">Authorization</span></span>  | <span data-ttu-id="c03bb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c03bb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c03bb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c03bb-129">Request body</span></span>
<span data-ttu-id="c03bb-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c03bb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c03bb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c03bb-131">Response</span></span>

<span data-ttu-id="c03bb-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupSettingTemplate](../resources/groupsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c03bb-132">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c03bb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c03bb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c03bb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c03bb-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c03bb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c03bb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="c03bb-136">C#</span><span class="sxs-lookup"><span data-stu-id="c03bb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c03bb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c03bb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c03bb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c03bb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c03bb-139">Java</span><span class="sxs-lookup"><span data-stu-id="c03bb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c03bb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c03bb-140">Response</span></span>

<span data-ttu-id="c03bb-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c03bb-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
