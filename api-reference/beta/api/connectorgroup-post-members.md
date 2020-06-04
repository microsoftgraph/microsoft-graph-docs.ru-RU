---
title: Добавление соединителя в Коннекторграуп
description: Используйте этот API, чтобы добавить соединитель в Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: de3f64a0b1efec39497d2b6e4a24bc690539fe75
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555805"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="44b84-103">Добавление соединителя в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="44b84-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="44b84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44b84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44b84-105">Добавление [соединителя](../resources/connector.md) в [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="44b84-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="44b84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44b84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44b84-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44b84-108">Permission type</span></span>      | <span data-ttu-id="44b84-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44b84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44b84-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44b84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44b84-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44b84-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44b84-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44b84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44b84-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44b84-113">Not supported.</span></span>    |
|<span data-ttu-id="44b84-114">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="44b84-114">Application</span></span> | <span data-ttu-id="44b84-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b84-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44b84-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44b84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="44b84-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44b84-117">Request headers</span></span>
| <span data-ttu-id="44b84-118">Имя</span><span class="sxs-lookup"><span data-stu-id="44b84-118">Name</span></span>       | <span data-ttu-id="44b84-119">Описание</span><span class="sxs-lookup"><span data-stu-id="44b84-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44b84-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="44b84-120">Authorization</span></span>  | <span data-ttu-id="44b84-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="44b84-121">Bearer.</span></span> <span data-ttu-id="44b84-122">Обязательное</span><span class="sxs-lookup"><span data-stu-id="44b84-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="44b84-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44b84-123">Request body</span></span>
<span data-ttu-id="44b84-124">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44b84-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="44b84-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="44b84-125">Response</span></span>

<span data-ttu-id="44b84-126">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44b84-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44b84-127">Пример</span><span class="sxs-lookup"><span data-stu-id="44b84-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44b84-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="44b84-128">Request</span></span>
<span data-ttu-id="44b84-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44b84-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
}
```
<span data-ttu-id="44b84-130">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44b84-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="44b84-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="44b84-131">Response</span></span>
<span data-ttu-id="44b84-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44b84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
