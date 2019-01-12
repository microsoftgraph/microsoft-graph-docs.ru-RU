---
title: Перечисление параметров группы
description: Получение списка, включающего объекты параметров группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8cb245c786ef1fbede3e305fd73df74eb574393c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932366"
---
# <a name="list-group-settings"></a><span data-ttu-id="90e8c-103">Перечисление параметров группы</span><span class="sxs-lookup"><span data-stu-id="90e8c-103">List group settings</span></span>

<span data-ttu-id="90e8c-104">Получение списка, включающего объекты параметров группы.</span><span class="sxs-lookup"><span data-stu-id="90e8c-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="90e8c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90e8c-105">Permissions</span></span>

<span data-ttu-id="90e8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90e8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="90e8c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90e8c-108">Permission type</span></span>      | <span data-ttu-id="90e8c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90e8c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90e8c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90e8c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90e8c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90e8c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90e8c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90e8c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90e8c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e8c-113">Not supported.</span></span>    |
|<span data-ttu-id="90e8c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90e8c-114">Application</span></span> | <span data-ttu-id="90e8c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e8c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90e8c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90e8c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="90e8c-117">Перечисление параметров на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="90e8c-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="90e8c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90e8c-118">Optional query parameters</span></span>
<span data-ttu-id="90e8c-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="90e8c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="90e8c-120">Примечание. $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e8c-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90e8c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90e8c-121">Request headers</span></span>
| <span data-ttu-id="90e8c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="90e8c-122">Name</span></span> | <span data-ttu-id="90e8c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="90e8c-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="90e8c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90e8c-124">Authorization</span></span>  | <span data-ttu-id="90e8c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90e8c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90e8c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90e8c-127">Request body</span></span>
<span data-ttu-id="90e8c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90e8c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90e8c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90e8c-129">Response</span></span>

<span data-ttu-id="90e8c-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="90e8c-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90e8c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90e8c-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="90e8c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90e8c-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="90e8c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="90e8c-133">Response</span></span>

<span data-ttu-id="90e8c-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90e8c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
