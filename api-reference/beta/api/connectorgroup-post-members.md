---
title: Добавление соединителя connectorGroup
description: Используйте этот интерфейс API для добавления соединитель connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 8df6fdda80007217164f8ae2f21a1d3f8d667d23
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518256"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="47b47-103">Добавление соединителя connectorGroup</span><span class="sxs-lookup"><span data-stu-id="47b47-103">Add connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47b47-104">Используйте этот интерфейс API для добавления соединитель connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="47b47-104">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="47b47-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47b47-105">Permissions</span></span>
<span data-ttu-id="47b47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47b47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47b47-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47b47-108">Permission type</span></span>      | <span data-ttu-id="47b47-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47b47-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47b47-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47b47-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47b47-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47b47-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47b47-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47b47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47b47-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47b47-113">Not supported.</span></span>    |
|<span data-ttu-id="47b47-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47b47-114">Application</span></span> | <span data-ttu-id="47b47-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47b47-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47b47-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47b47-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="47b47-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47b47-117">Request headers</span></span>
| <span data-ttu-id="47b47-118">Имя</span><span class="sxs-lookup"><span data-stu-id="47b47-118">Name</span></span>       | <span data-ttu-id="47b47-119">Описание</span><span class="sxs-lookup"><span data-stu-id="47b47-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47b47-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="47b47-120">Authorization</span></span>  | <span data-ttu-id="47b47-121">Токен носителя.</span><span class="sxs-lookup"><span data-stu-id="47b47-121">Bearer.</span></span> <span data-ttu-id="47b47-122">Обязательный</span><span class="sxs-lookup"><span data-stu-id="47b47-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="47b47-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47b47-123">Request body</span></span>
<span data-ttu-id="47b47-124">В тексте запроса укажите представление JSON ссылка на объект [соединителя](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="47b47-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="47b47-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="47b47-125">Response</span></span>

<span data-ttu-id="47b47-126">Успешно завершена, этот метод возвращает `201 Created` объект [соединителя](../resources/connector.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47b47-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47b47-127">Пример</span><span class="sxs-lookup"><span data-stu-id="47b47-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47b47-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="47b47-128">Request</span></span>
<span data-ttu-id="47b47-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47b47-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="47b47-130">В тексте запроса укажите представление JSON ссылка на объект [соединителя](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="47b47-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="47b47-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="47b47-131">Response</span></span>
<span data-ttu-id="47b47-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="47b47-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
