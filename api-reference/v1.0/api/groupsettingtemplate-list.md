---
title: Перечисление объектов groupSettingTemplate
description: Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d592b3e9ae084223a08364c7cd719e2b6d03c0ef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577807"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="2ab28-104">Перечисление объектов groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2ab28-104">List groupSettingTemplates</span></span>

<span data-ttu-id="2ab28-p102">Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="2ab28-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ab28-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ab28-107">Permissions</span></span>

<span data-ttu-id="2ab28-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ab28-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2ab28-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ab28-110">Permission type</span></span>      | <span data-ttu-id="2ab28-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ab28-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ab28-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ab28-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ab28-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ab28-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ab28-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ab28-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ab28-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab28-115">Not supported.</span></span>    |
|<span data-ttu-id="2ab28-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ab28-116">Application</span></span> | <span data-ttu-id="2ab28-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab28-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ab28-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ab28-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2ab28-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2ab28-119">Optional query parameters</span></span>
<span data-ttu-id="2ab28-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2ab28-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="2ab28-121">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab28-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ab28-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ab28-122">Request headers</span></span>
| <span data-ttu-id="2ab28-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2ab28-123">Name</span></span> | <span data-ttu-id="2ab28-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2ab28-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="2ab28-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ab28-125">Authorization</span></span>  | <span data-ttu-id="2ab28-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ab28-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ab28-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ab28-128">Request body</span></span>
<span data-ttu-id="2ab28-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ab28-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ab28-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ab28-130">Response</span></span>

<span data-ttu-id="2ab28-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupSettingTemplate](../resources/groupsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ab28-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab28-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2ab28-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ab28-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ab28-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="2ab28-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ab28-134">Response</span></span>

<span data-ttu-id="2ab28-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ab28-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
