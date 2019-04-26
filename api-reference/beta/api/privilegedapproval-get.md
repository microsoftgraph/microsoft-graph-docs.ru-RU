---
title: Получение privilegedApproval
description: Получение свойств и связей объекта привилежедаппровал.
localization_priority: Normal
ms.openlocfilehash: 976efcba63e0cf426d1838b84749b0afd4116aee
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332062"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="5c416-103">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5c416-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c416-104">Получение свойств и связей объекта привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="5c416-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c416-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c416-105">Permissions</span></span>
<span data-ttu-id="5c416-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c416-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5c416-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c416-108">Permission type</span></span>      | <span data-ttu-id="5c416-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c416-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c416-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c416-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c416-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="5c416-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="5c416-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c416-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c416-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c416-113">Not supported.</span></span>    |
|<span data-ttu-id="5c416-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c416-114">Application</span></span> | <span data-ttu-id="5c416-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c416-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c416-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c416-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c416-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c416-117">Optional query parameters</span></span>
<span data-ttu-id="5c416-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c416-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c416-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c416-119">Request headers</span></span>
| <span data-ttu-id="5c416-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5c416-120">Name</span></span>      |<span data-ttu-id="5c416-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5c416-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c416-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c416-122">Authorization</span></span>  | <span data-ttu-id="5c416-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c416-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c416-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c416-125">Request body</span></span>
<span data-ttu-id="5c416-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c416-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c416-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c416-127">Response</span></span>

<span data-ttu-id="5c416-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c416-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="5c416-129">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="5c416-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5c416-130">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="5c416-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="5c416-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5c416-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c416-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c416-132">Request</span></span>
<span data-ttu-id="5c416-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c416-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="5c416-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c416-134">Response</span></span>
<span data-ttu-id="5c416-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c416-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
