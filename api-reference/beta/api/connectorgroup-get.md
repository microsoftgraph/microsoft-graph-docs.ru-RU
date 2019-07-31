---
title: Получение Коннекторграуп
description: Получение свойств объекта Коннекторграуп.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ac1a8ff709b3795fa4491fca1b75b26ca2b9e138
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943486"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="8629e-103">Получение Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="8629e-103">Get connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8629e-104">Получение свойств объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="8629e-104">Retrieve the properties of a connectorGroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8629e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8629e-105">Permissions</span></span>
<span data-ttu-id="8629e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8629e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8629e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8629e-108">Permission type</span></span>      | <span data-ttu-id="8629e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8629e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8629e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8629e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8629e-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8629e-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8629e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8629e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8629e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8629e-113">Not supported.</span></span>    |
|<span data-ttu-id="8629e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8629e-114">Application</span></span> | <span data-ttu-id="8629e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8629e-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8629e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8629e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8629e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8629e-117">Optional query parameters</span></span>
<span data-ttu-id="8629e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8629e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8629e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8629e-119">Request headers</span></span>
| <span data-ttu-id="8629e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8629e-120">Name</span></span>      |<span data-ttu-id="8629e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8629e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8629e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8629e-122">Authorization</span></span>  | <span data-ttu-id="8629e-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="8629e-123">Bearer.</span></span> <span data-ttu-id="8629e-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8629e-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="8629e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8629e-125">Request body</span></span>
<span data-ttu-id="8629e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8629e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8629e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="8629e-127">Response</span></span>

<span data-ttu-id="8629e-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8629e-128">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8629e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8629e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8629e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8629e-130">Request</span></span>
<span data-ttu-id="8629e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8629e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="8629e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8629e-132">Response</span></span>
<span data-ttu-id="8629e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8629e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
