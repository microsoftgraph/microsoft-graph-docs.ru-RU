---
title: Получение шаблона параметров группы
description: Шаблон параметров группы представляет шаблон параметров, на базе которого в клиенте можно создавать параметры. Эта операция позволяет получить свойства объекта groupSettingTemplate, включая доступные параметры и их значения по умолчанию.
localization_priority: Normal
ms.openlocfilehash: 17e385c564337fcaa1255685e2b5808caec5cba4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805000"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="186a6-104">Получение шаблона параметров группы</span><span class="sxs-lookup"><span data-stu-id="186a6-104">Get a group setting template</span></span>

<span data-ttu-id="186a6-p102">Шаблон параметров группы представляет шаблон параметров, на базе которого в клиенте можно создавать параметры. Эта операция позволяет получить свойства объекта [groupSettingTemplate](../resources/groupsettingtemplate.md), включая доступные параметры и их значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="186a6-p102">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="186a6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="186a6-107">Permissions</span></span>

<span data-ttu-id="186a6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="186a6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="186a6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="186a6-110">Permission type</span></span>      | <span data-ttu-id="186a6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="186a6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="186a6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="186a6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="186a6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="186a6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="186a6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="186a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="186a6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="186a6-115">Not supported.</span></span>    |
|<span data-ttu-id="186a6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="186a6-116">Application</span></span> | <span data-ttu-id="186a6-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="186a6-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="186a6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="186a6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="186a6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="186a6-119">Optional query parameters</span></span>
<span data-ttu-id="186a6-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="186a6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="186a6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="186a6-121">Request headers</span></span>
| <span data-ttu-id="186a6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="186a6-122">Name</span></span> | <span data-ttu-id="186a6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="186a6-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="186a6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="186a6-124">Authorization</span></span> | <span data-ttu-id="186a6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="186a6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="186a6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="186a6-127">Request body</span></span>
<span data-ttu-id="186a6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="186a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="186a6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="186a6-129">Response</span></span>

<span data-ttu-id="186a6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [groupSettingTemplate](../resources/groupsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="186a6-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="186a6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="186a6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="186a6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="186a6-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="186a6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="186a6-133">Response</span></span>

<span data-ttu-id="186a6-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="186a6-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
