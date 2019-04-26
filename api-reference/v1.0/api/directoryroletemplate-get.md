---
title: Вывод объекта directoryRoleTemplate
description: Получение свойств и связей объекта directoryRoleTemplate.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d66cf5f4d8784eeee5d4f84dd4eaa3616bafa5a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562428"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="83c29-103">Вывод объекта directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="83c29-103">Get directoryRoleTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83c29-104">Получение свойств и связей объекта directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="83c29-104">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="83c29-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83c29-105">Permissions</span></span>
<span data-ttu-id="83c29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83c29-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83c29-108">Permission type</span></span>      | <span data-ttu-id="83c29-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83c29-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83c29-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83c29-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83c29-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83c29-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83c29-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83c29-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83c29-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83c29-113">Not supported.</span></span>    |
|<span data-ttu-id="83c29-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83c29-114">Application</span></span> | <span data-ttu-id="83c29-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83c29-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83c29-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83c29-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83c29-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="83c29-117">Optional query parameters</span></span>
<span data-ttu-id="83c29-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="83c29-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="83c29-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83c29-119">Request headers</span></span>
| <span data-ttu-id="83c29-120">Имя</span><span class="sxs-lookup"><span data-stu-id="83c29-120">Name</span></span>       | <span data-ttu-id="83c29-121">Тип</span><span class="sxs-lookup"><span data-stu-id="83c29-121">Type</span></span> | <span data-ttu-id="83c29-122">Описание</span><span class="sxs-lookup"><span data-stu-id="83c29-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="83c29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83c29-123">Authorization</span></span>  | <span data-ttu-id="83c29-124">string</span><span class="sxs-lookup"><span data-stu-id="83c29-124">string</span></span>  | <span data-ttu-id="83c29-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83c29-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83c29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83c29-127">Request body</span></span>
<span data-ttu-id="83c29-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83c29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83c29-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="83c29-129">Response</span></span>

<span data-ttu-id="83c29-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="83c29-130">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83c29-131">Пример</span><span class="sxs-lookup"><span data-stu-id="83c29-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83c29-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="83c29-132">Request</span></span>
<span data-ttu-id="83c29-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83c29-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="83c29-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="83c29-134">Response</span></span>
<span data-ttu-id="83c29-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83c29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
