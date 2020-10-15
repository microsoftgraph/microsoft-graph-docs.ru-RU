---
title: Перечисление объектов groupSettingTemplate
description: Получение списка доступных объектов Граупсеттингтемплатес.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a74edc3975ac85fabeaf59c1e34b064f35e8f510
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458376"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="ff8b2-103">Перечисление объектов groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="ff8b2-103">List groupSettingTemplates</span></span>

<span data-ttu-id="ff8b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff8b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff8b2-p101">Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="ff8b2-p101">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff8b2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff8b2-107">Permissions</span></span>

<span data-ttu-id="ff8b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff8b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ff8b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff8b2-110">Permission type</span></span>      | <span data-ttu-id="ff8b2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff8b2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff8b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff8b2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff8b2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff8b2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ff8b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff8b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff8b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff8b2-115">Not supported.</span></span>    |
|<span data-ttu-id="ff8b2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff8b2-116">Application</span></span> | <span data-ttu-id="ff8b2-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff8b2-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff8b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff8b2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ff8b2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff8b2-119">Optional query parameters</span></span>
<span data-ttu-id="ff8b2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ff8b2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="ff8b2-121">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff8b2-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff8b2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff8b2-122">Request headers</span></span>
| <span data-ttu-id="ff8b2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ff8b2-123">Name</span></span> | <span data-ttu-id="ff8b2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ff8b2-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ff8b2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff8b2-125">Authorization</span></span>  | <span data-ttu-id="ff8b2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff8b2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff8b2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff8b2-128">Request body</span></span>
<span data-ttu-id="ff8b2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff8b2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff8b2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff8b2-130">Response</span></span>

<span data-ttu-id="ff8b2-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupSettingTemplate](../resources/groupsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff8b2-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff8b2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ff8b2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff8b2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff8b2-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ff8b2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff8b2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="ff8b2-135">C#</span><span class="sxs-lookup"><span data-stu-id="ff8b2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff8b2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff8b2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff8b2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff8b2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff8b2-138">Java</span><span class="sxs-lookup"><span data-stu-id="ff8b2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ff8b2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff8b2-139">Response</span></span>

<span data-ttu-id="ff8b2-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff8b2-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
