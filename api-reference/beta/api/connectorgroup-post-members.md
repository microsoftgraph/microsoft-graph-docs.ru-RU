---
title: Добавление соединителя в Коннекторграуп
description: Используйте этот API, чтобы добавить соединитель в Коннекторграуп.
localization_priority: Normal
ms.openlocfilehash: 839189b323318b440608b699864a36b69a6c840d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327679"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="7e7ea-103">Добавление соединителя в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="7e7ea-103">Add connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e7ea-104">Используйте этот API, чтобы добавить соединитель в Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="7e7ea-104">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e7ea-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e7ea-105">Permissions</span></span>
<span data-ttu-id="7e7ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e7ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e7ea-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e7ea-108">Permission type</span></span>      | <span data-ttu-id="7e7ea-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e7ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e7ea-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e7ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e7ea-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e7ea-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e7ea-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e7ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e7ea-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e7ea-113">Not supported.</span></span>    |
|<span data-ttu-id="7e7ea-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="7e7ea-114">Application</span></span> | <span data-ttu-id="7e7ea-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e7ea-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e7ea-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e7ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7e7ea-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e7ea-117">Request headers</span></span>
| <span data-ttu-id="7e7ea-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7e7ea-118">Name</span></span>       | <span data-ttu-id="7e7ea-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7e7ea-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7e7ea-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e7ea-120">Authorization</span></span>  | <span data-ttu-id="7e7ea-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="7e7ea-121">Bearer.</span></span> <span data-ttu-id="7e7ea-122">Обязательный</span><span class="sxs-lookup"><span data-stu-id="7e7ea-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e7ea-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e7ea-123">Request body</span></span>
<span data-ttu-id="7e7ea-124">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e7ea-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e7ea-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e7ea-125">Response</span></span>

<span data-ttu-id="7e7ea-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e7ea-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e7ea-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7e7ea-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e7ea-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e7ea-128">Request</span></span>
<span data-ttu-id="7e7ea-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e7ea-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="7e7ea-130">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e7ea-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7e7ea-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e7ea-131">Response</span></span>
<span data-ttu-id="7e7ea-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e7ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
