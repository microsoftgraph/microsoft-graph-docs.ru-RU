---
title: Создание connectorGroup
description: Используйте этот интерфейс API для создания нового connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 233a80366c89b8cba31bd24e5d69b3a83fc20d1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509450"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="c2ccd-103">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="c2ccd-103">Create connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2ccd-104">Используйте этот интерфейс API для создания нового connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="c2ccd-104">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2ccd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ccd-105">Permissions</span></span>
<span data-ttu-id="c2ccd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2ccd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ccd-108">Permission type</span></span>      | <span data-ttu-id="c2ccd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2ccd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2ccd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2ccd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2ccd-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2ccd-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2ccd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2ccd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2ccd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2ccd-113">Not supported.</span></span>    |
|<span data-ttu-id="c2ccd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2ccd-114">Application</span></span> | <span data-ttu-id="c2ccd-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ccd-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2ccd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2ccd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="c2ccd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2ccd-117">Request headers</span></span>
| <span data-ttu-id="c2ccd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c2ccd-118">Name</span></span>       | <span data-ttu-id="c2ccd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c2ccd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c2ccd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2ccd-120">Authorization</span></span>  | <span data-ttu-id="c2ccd-121">Токен носителя.</span><span class="sxs-lookup"><span data-stu-id="c2ccd-121">Bearer.</span></span> <span data-ttu-id="c2ccd-122">Ли</span><span class="sxs-lookup"><span data-stu-id="c2ccd-122">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2ccd-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2ccd-123">Request body</span></span>
<span data-ttu-id="c2ccd-124">В тексте запроса укажите представление JSON объекта [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c2ccd-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c2ccd-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2ccd-125">Response</span></span>

<span data-ttu-id="c2ccd-126">Успешно завершена, этот метод возвращает `201 Created` объект [connectorGroup](../resources/connectorgroup.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2ccd-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2ccd-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c2ccd-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2ccd-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2ccd-128">Request</span></span>
<span data-ttu-id="c2ccd-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2ccd-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```
<span data-ttu-id="c2ccd-130">В тексте запроса укажите представление JSON объекта [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c2ccd-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c2ccd-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2ccd-131">Response</span></span>
<span data-ttu-id="c2ccd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c2ccd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-post-connectorgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
