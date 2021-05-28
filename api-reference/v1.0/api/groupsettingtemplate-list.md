---
title: Перечисление объектов groupSettingTemplate
description: Извлечение списка доступных объектов groupSettingTemplates.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 85ec50ce39f1bb98a3566b5e48daeec627dbf751
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679535"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="9a8fe-103">Перечисление объектов groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9a8fe-103">List groupSettingTemplates</span></span>

<span data-ttu-id="9a8fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a8fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a8fe-p101">Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="9a8fe-p101">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a8fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a8fe-107">Permissions</span></span>

<span data-ttu-id="9a8fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a8fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9a8fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a8fe-110">Permission type</span></span>      | <span data-ttu-id="9a8fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a8fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a8fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a8fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a8fe-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a8fe-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a8fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a8fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a8fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a8fe-115">Not supported.</span></span>    |
|<span data-ttu-id="9a8fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a8fe-116">Application</span></span> | <span data-ttu-id="9a8fe-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8fe-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a8fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a8fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a8fe-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9a8fe-119">Optional query parameters</span></span>
<span data-ttu-id="9a8fe-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9a8fe-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="9a8fe-121">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a8fe-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a8fe-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a8fe-122">Request headers</span></span>
| <span data-ttu-id="9a8fe-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9a8fe-123">Name</span></span> | <span data-ttu-id="9a8fe-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9a8fe-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="9a8fe-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a8fe-125">Authorization</span></span>  | <span data-ttu-id="9a8fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a8fe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a8fe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a8fe-128">Request body</span></span>
<span data-ttu-id="9a8fe-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a8fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a8fe-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a8fe-130">Response</span></span>

<span data-ttu-id="9a8fe-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupSettingTemplate](../resources/groupsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a8fe-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a8fe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9a8fe-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a8fe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a8fe-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9a8fe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a8fe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="9a8fe-135">C#</span><span class="sxs-lookup"><span data-stu-id="9a8fe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a8fe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a8fe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a8fe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a8fe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a8fe-138">Java</span><span class="sxs-lookup"><span data-stu-id="9a8fe-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a8fe-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a8fe-139">Response</span></span>

<span data-ttu-id="9a8fe-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9a8fe-140">Note: The response object shown here might be shortened for readability.</span></span>
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
