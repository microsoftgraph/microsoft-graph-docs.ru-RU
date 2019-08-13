---
title: Получение шаблона параметров группы
description: Шаблон параметров группы представляет шаблон параметров, параметры которых могут создаваться в клиенте. Эта операция позволяет получать свойства объекта groupSettingTemplate, включая доступные параметры и их значения по умолчанию.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b905c8bb905478ac580b13e47cb6e6118154c2b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364987"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="50f4b-104">Получение шаблона параметров группы</span><span class="sxs-lookup"><span data-stu-id="50f4b-104">Get a group setting template</span></span>

<span data-ttu-id="50f4b-p102">Шаблон параметров группы представляет шаблон параметров, на базе которого в клиенте можно создавать параметры. Эта операция позволяет получить свойства объекта [groupSettingTemplate](../resources/groupsettingtemplate.md), включая доступные параметры и их значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="50f4b-p102">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="50f4b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50f4b-107">Permissions</span></span>

<span data-ttu-id="50f4b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50f4b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="50f4b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50f4b-110">Permission type</span></span>      | <span data-ttu-id="50f4b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50f4b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50f4b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50f4b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50f4b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50f4b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50f4b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50f4b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50f4b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50f4b-115">Not supported.</span></span>    |
|<span data-ttu-id="50f4b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50f4b-116">Application</span></span> | <span data-ttu-id="50f4b-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50f4b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50f4b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50f4b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50f4b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50f4b-119">Optional query parameters</span></span>
<span data-ttu-id="50f4b-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50f4b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50f4b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50f4b-121">Request headers</span></span>
| <span data-ttu-id="50f4b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="50f4b-122">Name</span></span> | <span data-ttu-id="50f4b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="50f4b-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="50f4b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50f4b-124">Authorization</span></span> | <span data-ttu-id="50f4b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50f4b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50f4b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50f4b-127">Request body</span></span>
<span data-ttu-id="50f4b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50f4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50f4b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="50f4b-129">Response</span></span>

<span data-ttu-id="50f4b-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [groupSettingTemplate](../resources/groupsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="50f4b-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50f4b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="50f4b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50f4b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="50f4b-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="50f4b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="50f4b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="50f4b-134">C#</span><span class="sxs-lookup"><span data-stu-id="50f4b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50f4b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50f4b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50f4b-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="50f4b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="50f4b-137">Java</span><span class="sxs-lookup"><span data-stu-id="50f4b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50f4b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="50f4b-138">Response</span></span>

<span data-ttu-id="50f4b-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50f4b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1341

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates/$entity",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
