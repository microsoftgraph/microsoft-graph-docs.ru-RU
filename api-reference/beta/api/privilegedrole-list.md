---
title: Список privilegedRoles
description: Получение списка объектов privilegedRole.
localization_priority: Normal
ms.openlocfilehash: d954cedbaf4b164fe0649a3565ea0212d148c322
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518081"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="8d5b3-103">Список privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="8d5b3-103">List privilegedRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d5b3-104">Получение списка объектов [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="8d5b3-104">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="8d5b3-105">Чтобы отфильтровать результаты запроса, используйте стандартные OData ``$filter`` выражения в URI.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d5b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d5b3-106">Permissions</span></span>
<span data-ttu-id="8d5b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d5b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8d5b3-109">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="8d5b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d5b3-110">Permission type</span></span>      | <span data-ttu-id="8d5b3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d5b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d5b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d5b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d5b3-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d5b3-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d5b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d5b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d5b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-115">Not supported.</span></span>    |
|<span data-ttu-id="8d5b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d5b3-116">Application</span></span> | <span data-ttu-id="8d5b3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d5b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d5b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d5b3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d5b3-119">Optional query parameters</span></span>
<span data-ttu-id="8d5b3-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d5b3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d5b3-121">Request headers</span></span>
| <span data-ttu-id="8d5b3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8d5b3-122">Name</span></span>      |<span data-ttu-id="8d5b3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8d5b3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8d5b3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d5b3-124">Authorization</span></span>  | <span data-ttu-id="8d5b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d5b3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d5b3-127">Request body</span></span>
<span data-ttu-id="8d5b3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d5b3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d5b3-129">Response</span></span>

<span data-ttu-id="8d5b3-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedRole](../resources/privilegedrole.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="8d5b3-131">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8d5b3-132">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8d5b3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8d5b3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d5b3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d5b3-134">Request</span></span>
<span data-ttu-id="8d5b3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d5b3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
##### <a name="response"></a><span data-ttu-id="8d5b3-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d5b3-136">Response</span></span>
<span data-ttu-id="8d5b3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8d5b3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
