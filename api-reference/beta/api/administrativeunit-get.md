---
title: Получение administrativeUnit
description: Извлечение свойств и связи объекта administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 588d116d546503fa8db6c8ba56c5d0e328a10b8a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521609"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="f9a1a-103">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="f9a1a-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9a1a-104">Извлечение свойств и связи объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="f9a1a-104">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="f9a1a-105">Поскольку ресурсов **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), вы также можете использовать `GET` операции для получения данных расширения и настраиваемых свойств в экземпляре **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="f9a1a-105">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9a1a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9a1a-106">Permissions</span></span>
<span data-ttu-id="f9a1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9a1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f9a1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9a1a-109">Permission type</span></span>      | <span data-ttu-id="f9a1a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9a1a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9a1a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9a1a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9a1a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9a1a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f9a1a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9a1a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9a1a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9a1a-114">Not supported.</span></span>    |
|<span data-ttu-id="f9a1a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9a1a-115">Application</span></span> | <span data-ttu-id="f9a1a-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9a1a-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9a1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9a1a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9a1a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9a1a-118">Optional query parameters</span></span>
<span data-ttu-id="f9a1a-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9a1a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9a1a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9a1a-120">Request headers</span></span>
| <span data-ttu-id="f9a1a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f9a1a-121">Name</span></span>      |<span data-ttu-id="f9a1a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f9a1a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9a1a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9a1a-123">Authorization</span></span>  | <span data-ttu-id="f9a1a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9a1a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9a1a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9a1a-126">Request body</span></span>
<span data-ttu-id="f9a1a-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9a1a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9a1a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9a1a-128">Response</span></span>

<span data-ttu-id="f9a1a-129">Успешно завершена, этот метод возвращает `200 OK` объект [administrativeUnit](../resources/administrativeunit.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9a1a-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9a1a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f9a1a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9a1a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9a1a-131">Request</span></span>
<span data-ttu-id="f9a1a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9a1a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="f9a1a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9a1a-133">Response</span></span>
<span data-ttu-id="f9a1a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f9a1a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="f9a1a-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f9a1a-137">See also</span></span>

- [<span data-ttu-id="f9a1a-138">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="f9a1a-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f9a1a-139">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f9a1a-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
