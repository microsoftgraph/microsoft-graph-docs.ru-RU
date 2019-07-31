---
title: Добавление соединителя в Коннекторграуп
description: Используйте этот API, чтобы добавить соединитель в Коннекторграуп.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c8b428ca6c724ce37116430cbae56587866c13eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943388"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="9e27e-103">Добавление соединителя в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="9e27e-103">Add connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e27e-104">Используйте этот API, чтобы добавить соединитель в Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="9e27e-104">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e27e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e27e-105">Permissions</span></span>
<span data-ttu-id="9e27e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e27e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e27e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e27e-108">Permission type</span></span>      | <span data-ttu-id="9e27e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e27e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e27e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e27e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e27e-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e27e-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e27e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e27e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e27e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e27e-113">Not supported.</span></span>    |
|<span data-ttu-id="9e27e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e27e-114">Application</span></span> | <span data-ttu-id="9e27e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e27e-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e27e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e27e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9e27e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e27e-117">Request headers</span></span>
| <span data-ttu-id="9e27e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9e27e-118">Name</span></span>       | <span data-ttu-id="9e27e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9e27e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9e27e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e27e-120">Authorization</span></span>  | <span data-ttu-id="9e27e-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="9e27e-121">Bearer.</span></span> <span data-ttu-id="9e27e-122">Обязательный</span><span class="sxs-lookup"><span data-stu-id="9e27e-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e27e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e27e-123">Request body</span></span>
<span data-ttu-id="9e27e-124">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e27e-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9e27e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e27e-125">Response</span></span>

<span data-ttu-id="9e27e-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e27e-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e27e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="9e27e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e27e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e27e-128">Request</span></span>
<span data-ttu-id="9e27e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e27e-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connector/{id}"
}
```
<span data-ttu-id="9e27e-130">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e27e-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9e27e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e27e-131">Response</span></span>
<span data-ttu-id="9e27e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e27e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
